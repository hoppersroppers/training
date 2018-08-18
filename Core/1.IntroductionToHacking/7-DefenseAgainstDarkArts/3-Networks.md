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
 
If you make a request to a website or send/recieve any data across the internet, you have given your router's IP address. This request can take any form, from a visiting a link, viewing an image hosted there, or being redirected through a short link. You can also be tricked into opening a file that sends a request out to the internet, running a program which profiles your computer and sends out a request, or even running a terrible DDOS tool that makes no attempt to hide that it is running on your own network. An attacker can use these requests to identify someone through a 3rd party service. 
 
 Tasks:
 * Visit http://www.whatsmyip.org/more-info-about-you/
 * How much information did they know about you?
 * Use this site to shorten a URL and get your IP https://iplogger.org/shortener/
 * Use this site to create a hidden image to get your IP. Send it to yourself via email. https://iplogger.org/invisible/. 
 * Visit: https://canarytokens.org/generate and make various tokens to be used for getting IP addresses and try them on yourself
    * Word Document 
    * Custom Image
    
 
 Now to add what is called a proxy. Basically, this is a server you send a request to that routes all the traffic through them first, then passes it on to you. The critical thing to remember is that this extra hop added by the proxy, although it obfuscates your IP from the end target, does not hide it from the servers providing the service. They can see all of your traffic, and can do whatever they want with it. Your extra hops will create logs, and all those logs can still be used if someone gets them.
 
Tasks:
* Visit https://hide.me/en/proxy
* Use their proxy to visit http://www.whatsmyip.org/more-info-about-you/
* How much information do they have about you now?

Adding an extra hop works, but it needs to be done intelligently, and certainly not through a sketchy website which provides it for free. 
    
## Hiding Your IP and Circumventing Censorship


So now we know we need to add something in between ourselves and the things we are trying to visit. There are a varieties of ways to do that, but the most important bit is that we are able to trust the hops we are using, because a malicious hop is almost as bad as no hop at all. 

First, some vocab.
* Port Forward
* Proxy
* Proxychains
* VPNs
* TOR

 * https://danielmiessler.com/study/internet-deep-dark-web
 
 Tasks: 
 * Make Your Own Proxy
 * Make your own proxychains
 * Setup your own VPN
 * Don't go on TOR. Tis a silly place.
 
       
## Circumventing Proxies and Going Right to the Source

Remember honey tokens? Or just malware. That calls home real nice. There's also a fine line in the middle refered to by some as a "Network Investigative Tool" which is basically just a system profiler that calls home and deletes itself.

## What Can Be Done with an IP
   * Identify general location BUT THAT IS ALL YOU CAN DO WITH AN IP ADDRESS.
   * DDOS their router 
   * Hacking their Router
   * Court orders to ISPs
   * Threaten to give it to police so they can go get a court order
   

## Encryption


Tasks:
* Read this: https://www.usna.edu/CyberDept/sy110/lec/cryptSymmEnc/lec.html
* What is symetric encryption?
* Do the HW: https://www.usna.edu/CyberDept/sy110/lec/cryptSymmEnc/hw/hw.pdf
* Read this: https://www.usna.edu/CyberDept/sy110/lec/cryptAsymmEnc/lec.html
* What is assymetric encryption?
* Do the HW: https://www.usna.edu/CyberDept/sy110/lec/cryptAsymmEnc/hw/hw.pdf

Read this: https://ssd.eff.org/en/module/what-encryption

Random note, that link goes to the Electronic Frontier Foundation's website, they are basically the people who maintain internet freedom and digital rights for the rest of us. Good folks.

Now here is a slightly more technical primer on how real world cryptography works.

Read this: https://ssd.eff.org/en/module/introduction-public-key-cryptography-and-pgp

Alright, now that you have an idea of what encryption is, read this https://danielmiessler.com/study/encoding-encryption-hashing-obfuscation/ and explain the differences between the ideas explained.

## Man in the Middle
What is a man in the middle attack? You may have heard this before, and you'll hear it plenty more as it is the easiest and most common network attack.

The general idea is that if Computer A tries to communicate with Computer C, but their conversation transits over Computer B, B is able to read and even alter the messages being sent. This can allow Computer B to impersonate both people to each other and have them each receive a totally incorrect message while never knowing that they are being listened in on. This was not a huge problem back in the '70s on ARPANET, but now, when there are dozens of hops between your computer and whatever website you visit, any of those could be intercepting your traffic (and mostly likely multiple are).

Once again, the academy's piece on this is pretty damn good. Of course, we'll be going into this deeper later and you will do it yourself, but it's a good speed intro.

https://www.usna.edu/CyberDept/sy110/lec/cryptSymmEnc/lec.html

Questions:
* Of CIANA, what were the pillars that can be attacked if an adversary is able to do a man in the middle?
* In the Computer A,B and C scenario, what are the human names which match up to them?
* This one requires a google, but who is Mallory, and what makes her different from Eve?
* How does your browser protect you from MITM attacks? This will require a google.

## How to Be Safe
* Use a VPN/proxy/tor
* Use https everywhere!
* ublock origin should alreayd be on
* Browser safety extensions!
* Basic wifi safety
    * Use a VPN!* Open WiFi vs. secure WiFi
    * http://fieldguide.gizmodo.com/how-to-stay-safe-on-public-wifi-1779464400
    * https://www.google.com/safetycenter/everyone/start/safe-networks/

# You weren't updated or the patch didn't come out fast enough

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
