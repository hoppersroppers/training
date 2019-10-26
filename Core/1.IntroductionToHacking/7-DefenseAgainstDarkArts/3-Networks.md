# Hostile Networks
## Intro
Add this to the list of security truisms.

"Any network connected to the internet must be considered hostile." Most intranets should be considered hostile too. In fact, it is hard to imagine a more "hostile" network than a DoD network.

But what does "hostile" mean? In this case, the general idea is that if computer A wishes to communicate with computer C, that means that they need to send all of their traffic through computer B. Gentleman's agreements not to look at that traffic might have worked on Arpanet, but not anymore.

From Internet Service Providers (ISPs) working with governments to snoop on all your traffic, to deep sea submarine cable intercepts to sketchy free wifi hotspots, your internet browsing is recorded by a lot of people. And when I mean, a lot of people, I mean literally every single hop on your way across the internet (remember traceroute?) will have a complete log of your connections. They might not have the content if you have encrypted your traffic, but they will have records of the date/time the request was made, from who, and to where. This is accessible to anyone with access to the logs, whether they own it, pwned it, or have a court order. Your IP address is likely shared, but if logs are kept all the way down, and they likely do exist, anything can be tracked down to you.

This next section skips over the technical details of network ownage (while giving you plenty to research on your own time), and focuses on the principles that can protect you and specific steps you can take to protect yourself.

Recommended Listening: The Hostile Gospel, Talib Kweli <https://www.youtube.com/watch?v=_c5mDTq3sgo>



## Don't Give Out Your IP

If you make a request to a website or send/receive any data across the internet, you have given your router's IP address. This request can take any form, from a visiting a link, viewing an image hosted there, or being redirected through a short link.

 Tasks:
 * Visit <https://www.whatsmyip.org/more-info-about-you/>
 * How much information did they know about you?
 * Use this site to shorten a URL and get your IP <https://iplogger.org/shortener/>
 * Use this site to create a hidden image to get your IP. Send it to yourself via email. <https://iplogger.org/invisible/. >

 This last hidden image is how most email tracking works! You are able to see every time someone opens an email, which is useful primarily for marketing folks, but also in general life. I used to have this on all my emails so I could track opens/forwards/when to send follow up emails, but after getting complaints about it being a privacy violation, I stopped. It was very useful when I used it, but out of respect for the people I email, I decided it wasn't worth it. Everything in security is a trade off, especially when it comes to tracking your users and other people. Tending towards the side of Do Not Track without explicit consent is always the way to go.

 # They got your IP address

 First, let's get back into threat modeling... If you are doing something so 'fun' that if someone was able to provably demonstrate that you were the one behind the keyboard at the time you would go to jail or worse, this is the most important of all the sections. But you hopefully don't fall into this category, and more likely are worried about online censorship, aka web content filters. Luckily proxies help with both  problems.

 So while we mostly care about circumventing censorship, we will also teach as if you had to care about bad guys getting your IP address.
 It's a good thing to know. It is also a good thing to know in the event that you get a bad guys IP address. There are a lot of things to do with that.

 But first, you must understand that when someone "has" someone's IP address across the internet, they really just have the address of their gateway router. Whether this IP is from a website access or by requesting the logs of who owns a 3rd party provider account, not much can be done with this information yet. This allows the identification of the Internet Service Provider and the general location that service is provided to, which will usually provide the correct city. In order to get any more specific, law enforcement would need to be notified and LE would send a request would need to be sent to the ISP for logs of what user was associated with that router at that time. If the ISP provides those logs, then LE would have to go on premise to where the router is located to pull the router logs and continue the investigation. Those logs would be used to identify the person in question who was associated with whatever activity was first identified as suspect. Without router logs, the investigators will have to seize all computers and do forensics on them in order to identify who is the target. If this is a large enough group of computers, the investigation will likely have to take a different route, most likely enabling logging on the router and hoping the target connects again.

 The other route that is possible is to directly hack the IP address associated with the gateway router, drop malware, and then infect the target once you have identified them off the local network. However, there are not many organizations that are allowed to do this, so... it probably isn't your highest priority. Expect the normal investigative path to be followed 99% of the time.
 Did this makes sense?

 1. Type up the investigative path for identifying someone who has sent a threatening email from a "@gmail.com" address.


## Hiding Your IP and Circumventing Censorship

    So now we know we need to add something in between ourselves and the things we are trying to visit. There are a varieties of ways to do that, but the most important bit is that we are able to trust the hops we are using, because a malicious hop is often times as bad as no hop at all.

     * <https://danielmiessler.com/study/internet-deep-dark-web>

    First, some vocab.

     Tasks:
    1. Define all the vocab words.
    * Port Forward
    * Proxy
    * Proxychains
    * VPNs
    * TOR
    * Dark Web
    * Deep Web

A proxy is a server you send a request to that routes all the traffic through them first, then passes it on to you. The critical thing to remember is that this extra hop added by the proxy, although it obfuscates your IP from the end target, does not hide it from the servers providing the service. The other primary benefit of a proxy is that it protects your traffic from being snooped on by your first couple hops off your network, because all data is encrypted and goes directly to the proxy server. This means you bypass all local content filtering, unless the local filters also block proxy servers, thus kicking off a cat and mouse game. You might already have a good idea of what proxies are from using them to play games on school computers.

 Even if the local hops can't see your traffic, the proxy server itself sees all of your traffic, and whoever runs the server can do whatever they want with it. This means that whoever runs your proxy has access to all your traffic. As a general rule, the more expensive the proxy, the better chance it is your data isn't being sold, because when the product is free, the product is you.

 Remember your extra hops will create logs, and all those logs can still be used if someone gets them. No company that runs a proxy will ignore a subpoena.

I am not going to get too into detail with TOR and dark web stuff on this course. Just know TOR can be used for good things and bad things, just like everything else in technology.

Tasks:
* Visit <https://hide.me/en/proxy>
* Use their proxy to visit <https://www.whatsmyip.org/more-info-about-you/>
1. How much information does whatsmyIP they have about you now?
2. How much information does hide.me have about you now?
3. How much information does your local network admin have about you?
   * Do they have local monitoring software on your computer?
   * How could a local network admin identify what site you just visited through a proxy?

Adding an extra hop works, but it needs to be done intelligently, and certainly not through a sketchy website which provides it for free. Also notable is that your proxy may leak some information, especially via DNS, but also through other complicated in-browser capabilities.

Use this site to check your device with and without a proxy.
* <https://ipleak.net/>
* Use hide.me again and check for leaks. You shouldn't see anything. However, most of your browser information should remain the same. This can still be used to fingerprint.

I am going to make you set up your own proxy at some point, but not yet.


## Circumventing Proxies and Going Right to the Source

You can also be tricked into opening a file that sends a request out to the internet or running a program which profiles your computer and sends out a request. An attacker can use these requests to identify the IP of someone through a 3rd party service, like Twitter or Facebook, and around a proxy.

One method of doing this is called a honeytoken. Honeytokens are documents that contain a URL requests which call back and give the IP of the host it is on upon access. Not only does this give the IP, it more importantly gives the defender notification that someone has the document. The point of the honeytoken is mainly to identify that someone has access to the document and it is time for them to begin incident response. Make some of your own honey docs to practice and see what it looks like. I used to use this for some of my documents I sent around to see what organizations were sharing my powerpoints. It was very useful.  

* Visit: <https://canarytokens.org/generate> and make various tokens to be used for getting IP addresses and try them on yourself
   * Word Document
   * Custom Image

Or attackers can just use malware. Malware calls home real nice. There's also a fine line in the middle referred to by some as a "Network Investigative Tool" which is basically just a system profiler that calls home and deletes itself used by Law Enforcement agencies.



## Encryption

So we are now using a proxy and all the hops in the middle before our proxy can't identify our traffic. This is because of encryption. Encryption is a fairly complicated concept, but is essential to understanding how the internet functions.

Tasks:
* Read this: <https://www.usna.edu/CyberDept/sy110/lec/cryptSymmEnc/lec.html>
* Read this: <https://www.usna.edu/CyberDept/sy110/lec/cryptAsymmEnc/lec.html>

1. What is symmetric encryption?
2. Do the HW: <https://www.usna.edu/CyberDept/sy110/lec/cryptSymmEnc/hw/hw.pdf>
3. What is asymmetric encryption?
4. Do the HW: <https://www.usna.edu/CyberDept/sy110/lec/cryptAsymmEnc/hw/hw.pdf>

Read this: <https://ssd.eff.org/en/module/what-encryption>

Random note, that link goes to the Electronic Frontier Foundation's website, they are basically the people who maintain internet freedom and digital rights for the rest of us. Good folks.

Now here is a slightly more technical primer on how real world cryptography works.

Read this: <https://ssd.eff.org/en/module/introduction-public-key-cryptography-and-pgp>

Alright, now that you have an idea of what encryption is, read this <https://danielmiessler.com/study/encoding-encryption-hashing-obfuscation/> and explain the differences between the ideas explained.

1. What is the difference between HTTP and HTTPS traffic?
2. What can a server on a hop between you and the site you are visiting see if you use HTTP?
3. What can a server see if you use HTTPS?
4. Read about and install the HTTPS Everywhere extension if you haven't already. <https://chrome.google.com/webstore/detail/https-everywhere/>


## Man in the Middle
What is a man in the middle attack? You may have heard this before, and you'll hear it plenty more as it is the easiest and most common network attack.

The general idea is that if Computer A tries to communicate with Computer C, but their conversation transits over Computer B, B is able to read and even alter the messages being sent. This can allow Computer B to impersonate both people to each other and have them each receive a totally incorrect message while never knowing that they are being listened in on. This was not a huge problem back in the '70s on ARPANET, but now, when there are dozens of hops between your computer and whatever website you visit, any of those could be intercepting your traffic (and mostly likely multiple are).

* <https://www.veracode.com/security/man-middle-attack>
* <https://doubleoctopus.com/blog/the-ultimate-guide-to-man-in-the-middle-mitm-attacks-and-how-to-prevent-them/>

Questions:
1. Of CIA, what were the pillars that can be attacked if an adversary is able to do a man in the middle?
2. Describe how a MITM works, in your own words.
3. What is SSL stripping?
4. What is Man in the Browser?
5. What is an Evil Twin attack?
6. How does your browser protect you from MITM attacks? This will require a google.

## How to Be Safe on Public Wifi
Public Wifi was, for a long time, the most dangerous thing to do other than use a public computer. With the rise of HTTPS it is less of a concern, but it is still important to protect yourself.
    * <https://fieldguide.gizmodo.com/how-to-stay-safe-on-public-wifi-1779464400>
    * <https://www.google.com/safetycenter/everyone/start/safe-networks/>

# You got Zero Day'd
First, what is a zero day? Often written 0 day, pronounced "oh day" (this is contentious but this is the way I say it and you should too) 0 days are exploits that have not been patched yet.
* <https://www.fireeye.com/current-threats/what-is-a-zero-day-exploit.html>

This is a good article. <https://www.forbes.com/sites/andygreenberg/2012/03/23/shopping-for-zero-days-an-price-list-for-hackers-secret-software-exploits/#4c1e46232660>

So there are people out there who write 0 days and sell them to people who broker 0 days who sell them to people who use 0 days but guess what... you're (probably) not important enough to be a target. See: threat modeling
* Here are some prices to give you an idea of things.
   *  <https://www.wired.com/2015/11/heres-a-spy-firms-price-list-for-secret-hacker-techniques/>
   *  <https://www.zerodium.com/program.html>

There are exploit writers and other developers out there who will find 0 days and will not use them maliciously, and instead report them to the software developers so they can be patched prior to someone else discovering it and exploiting it in the wild. The best known  example is Google Project Zero. <https://www.wired.com/2014/07/google-project-zero/>

# You weren't updated or the patch didn't come out fast enough
Now just because 0 days won't be used on you, doesn't mean you are safe from exploits. We are now going to get into a complex and very important subject for you to understand.

Upon the discovery of an 0 day by one party, they now have the ability to use it on any target because all targets are unpatched. Always remember, multiple parties can have the same 0 day if they independently develop it. In addition, upon first use of an 0 day, the person it has been used on and all hops in the network from attacker to defender have the ability to identify the exploit on the wire and begin reversing it. If a country or organization records and retains network traffic they have the potential to identify malware on a system, trace it back to a network attack, pull their logs, and then identify how the 0 day worked. Now they have the 0 day as well.

Now there are two options: they can repurpose the 0 day for their own use, or, they can report it to the software manufacturer so that they can patch the vulnerability. If they continue using the vuln, it remains an 0 day. If they report the vuln, it is still an 0 day but will only remain an 0 day until the patch is released. Once that patch is released, the vulnerability becomes an n-day, as in it has been patched for n days.

During this period of time it is critical to download the patch as quickly as possible, because malicious attackers are busy reverse engineering patches for major pieces of software in order to develop exploits for unpatched boxes. While some boxes cannot be patched for various reasons, the majority are not patched because people are lazy and do not install patches. Modern systems realize that you are more safe if updates occur automatically. There are very very few situations in which you cannot have auto update turned on. 99% of those situations involve Windows boxes running legacy critical systems. If you don't have auto update turned on... you need to fix that.

Android doesn't do a good job of releasing patches quickly, Apple does it very well. Don't worry too much about this, but it is something to be aware of.  

1. Ensure Auto Update on for everything, especially Chrome and Windows.
