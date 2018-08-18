# Hostile Networks
## Intro
Add this to the list of security truisms.

Any network connected to the internet must be considered hostile. Most intranets should be considered hostile to. In fact, it is hard to imagine a more "hostile" network than a DoD network.

But what does "hostile" mean? In this case, the general idea is that if computer A wishes to communicate with computer C, that means that they need to send all of their traffic through computer B. Gentleman's agreements not to look at that traffic might have worked on Arpanet, but not anymore.

From Internet Service Providers (ISPs) working with governments to snoop on all your traffic, to deep sea submarine cable intercepts to sketchy free wifi hotspots, your internet browsing is recorded by a lot of people. And when I mean, a lot of people, I mean literally every single hop on your way across the internet (remember traceroute?) will have a complete log of your connections. They might not have the content if you have encrypted your traffic, but they will have records of the date/time the request was made, from who, and to where. This is accesssible to anyone with access to the logs, whether they own it, pwned it, or have a court order. Your IP address is likely shared, but if logs are kept all the way down, and they likely do exist, anything can be tracked down to you.

This next section skips over the technical details of network ownage (while giving you plenty to research on your own time), and focuses on the principles that can protect you and specific steps you can take to protect yourself.

Recommended Listening: The Hostile Gospel, Talib Kweli

# They got your IP address

First, let's get into threat modeling... If you are doing something so 'fun' that if someone was able to provably demonstrate that you were the one behind the keyboard at the time you would go to jail or worse, this is the most important of all the sections. But you hopefully don't fall into this category, and more likely are worried about online censorship, aka web content filters. That's how I started. 

So while we mostly care about circumventing censorship, we will also teach as if you had to care about bad guys getting your IP address. 
It's a good thing to know.

## Don't Give Out Your IP
 
 If you make a request to a website, you have given them your IP address. This request can take any form, from a visiting a link, viewing an image hosted there, or being redirected through a short link. You can also be tricked into opening a file that sends a request out to the internet, running a program which profiles your computer and sends out a request, or even running a terrible DDOS tool that makes no attempt to hide that it is running on your own network. An attacker can use these requests to identify someone through a 3rd party service. 
 
 Tasks:
 * Visit http://www.whatsmyip.org/more-info-about-you/
 * How much information did they know about you?
 * Use this site to shorten a URL and get your IP https://iplogger.org/shortener/
 * Use this site to create a hidden image to get your IP. Send it to yourself via email. https://iplogger.org/invisible/. 
 * Visit: https://canarytokens.org/generate and make various tokens to be used for getting IP addresses and try them on yourself
    * Word Document 
    * Custom Image
    
## Hiding Your IP and Circumventing Censorship
   * Port Forwarding, Proxies, Proxychains, VPNs, TOR
       * https://danielmiessler.com/study/internet-deep-dark-web
       
## Circumventing Proxies and Going Right to the Source

Remember honey tokens?

## What Can Be Done with an IP
   * GeoIP
   * Hacking 
   * Court orders to ISPs
   

## Encryption

* Encoding
 * Encryption
    * Symetrical
	* https://www.usna.edu/CyberDept/sy110/lec/cryptSymmEnc/lec.html
    * Asymetrical
	 https://www.usna.edu/CyberDept/sy110/lec/cryptAsymmEnc/lec.html
	 How does encryption work? (It takes a long fucking time)


 * Hashing
    * https://www.usna.edu/CyberDept/sy110/lec/cryptHashPswd/lec.html
    * https://xkcd.com/936/
    * L0phtcrack tangent
	* http://www.washingtonpost.com/sf/business/2015/06/22/net-of-insecurity-part-3/?utm_term=.ea6927af0bd7
	* en.wikipedia.org/wiki/L0pht
	* Responsible Hacking

 * Password Cracking 
   * https://arstechnica.com/information-technology/2013/03/how-i-became-a-password-cracker/
   * crack Local static rar
   * use google to crack a hash
   * crack Remote w/ hydra
   * Talk about rocku	and linkedin and all sorts of others
   * TroyHunt and password database thing project
So we know the attacker is trying to read the message... what is the best way to stop that?

Read this: https://ssd.eff.org/en/module/what-encryption

Random note, that link goes to the Electronic Frontier Foundation's website, they are basically the people who maintain internet freedom and digital rights for the rest of us. Good folks.

Now here is a slightly more technical primer on how real world cryptography works.

https://ssd.eff.org/en/module/introduction-public-key-cryptography-and-pgp

## Man in the Middle
What is a man in the middle attack? You may have heard this before, and you'll hear it plenty more as it is the easiest and most common network attack.

The general idea is that if Computer A tries to communicate with Computer C, but their conversation transits over Computer B, B is able to read and even alter the messages being sent. This can allow Computer B to impersonate both people to each other and have them each receive a totally incorrect message while never knowing that they are being listened in on. This was not a huge problem back in the '70s on ARPANET, but now, when there are dozens of hops between your computer and whatever website you visit, any of those could be intercepting your traffic (and mostly likely multiple are).

Once again, the academy's piece on this is pretty damn good. Of course, we'll be going into this deeper, but it's a good speed intro.

https://www.usna.edu/CyberDept/sy110/lec/cryptSymmEnc/lec.html

Questions:

Of CIANA, what were the pillars that can be attacked if an adversary is able to do a man in the middle?

In the Computer A,B and C scenario, what are the human names which match up to them?

This one requires a google, but who is Mallory, and what makes her different from Eve?

## How to Be Safe
VPN/proxy/tor

https everywhere!
ublock origin should alreayd be on
Browser safety extensions!

https://danielmiessler.com/study/internet-deep-dark-web

Basic wifi safety
Use a VPN!* Open WiFi vs. secure WiFi
http://fieldguide.gizmodo.com/how-to-stay-safe-on-public-wifi-1779464400
https://www.google.com/safetycenter/everyone/start/safe-networks/
Nation state ownage
Threat modeling


# You weren't updated

* Modern systems realize that you are more safe if updates occur automatically. There are very very few situations in which you cannot have auto update turned on. 99% of those situations involve Windows boxes running legacy critical systems. If you don't have auto update turned on... you need to fix that.
* Turn it on for everything
* Android doesnt update well, apple does it very well. 

	

		 
# You got 0'Dayd
        * Guess what... you're not important enough for that. See: threat modeling
* Here are some prices
https://www.wired.com/2015/11/heres-a-spy-firms-price-list-for-secret-hacker-techniques/

https://www.zerodium.com/program.html

set flash click to play
Adobe Reader DC
Adobe Reader is actually pretty safe if you have the full suite of security settings turned on. In the case of Adobe Reader DC, there's just one setting you need to change:

Edit > Preferences > Security (Enhanced) > Protected View > Files from potentially unsafe locations

Remember thegrugq, from the opsec lessons? 

https://www.forbes.com/sites/andygreenberg/2012/03/23/shopping-for-zero-days-an-price-list-for-hackers-secret-software-exploits/#4c1e46232660
