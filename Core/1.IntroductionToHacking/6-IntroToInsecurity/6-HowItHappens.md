As we went over earlier, if a sufficiently advanced attacker wants to get into your stuff specifically, they will.

But we have looked at our threat model before and have determined we are probably not a person of interest to the NSA/Mossad/FSB, right? Right???

So according to our threat model, the most likely people to hack us will be random criminals who don't care who we are, they're just trying to get in. While it is an over simplification, "An ounce of prevention is worth a pound of cure". If you are able to harden yourself ahead of time and not be an easy target, you will be much less likely to get hit with a non-targeted attack, and in the possibility that you ever are targeted, you will be more likely to not get caught off guard.

These are all of the reasons you might get hacked. 

# You used a shitty password 
https://ssd.eff.org/en/module/creating-strong-passwords
 
Passwords are hard, and losing your primary email can pretty much stop your life as you attempt to regain control. Luckily, there is a lot you can do to keep yourself from becoming the low hanging fruit. After this section, not only will you be able to protect yourself, but you’ll be able to share this with others.

     * Read this
        * http://www.passwordanalytics.com/theory/passwords/
        * Read Passwords 101 and submit one example each of the three ways you authenticate yourself.
        * Read Good Passwords 101 and submit a description of what makes a good password
        * Read Strength 101 and submit a description of what makes a strong password
        * Read Pass-Phrase and describe how pass phrases balance being a good password and a strong password.
        * Read Cracking and explain which technique an attacker would use to attack a password that they knew to be 6 random alpha numeric characters
        * Read Cracking and explain which technique an attacker would use to attack a password that they knew to be three random words added together.
     * Why They Matter
        * Here is a brief experiment for you to try. Try to make a rough guess how many web sites you use on a regular basis use your primary email as their account recovery address. Now, try to think about which of those sites are the most important to you that they remain secure; social media, banking, other email accounts. Now think of the sketchy sites you reuse the same password on. If those sites are breached, and the attacker gets your password, they can use it to take your other accounts.
	
        * - Now, work through the _____ Risk Assessment Steps to determine the level of risk that you assume by reusing your password. 
        * Password Manager
        * All is not lost however, luckily you do not have to memorize hundreds of high entropy passwords or carry them around in a locked diary. Password managers provide the ability to generate and store secure passwords across devices, all controlled by a single master password. This means you only need to know one password, and the rest can be pseudo-randomly generated. 
        * Read this! 
           * https://www.howtogeek.com/141500/why-you-should-use-a-password-manager-and-how-to-get-started/
           * Submit a 2-3 sentence statement trying to convince my grandma to use a password manager.
		* Relevant XKCD https://www.explainxkcd.com/wiki/index.php/936#Explanation
		   * What password has 2^44 bits of entropy?

* Install LastPass https://lastpass.com/
* Submit a screenshot of something
* Complete the LastPass Security challenge
 
 Single Sign On Awareness
  
  What is multi factor authentication?
       

   Multifactor authentication
   https://www.cs.cornell.edu/courses/cs513/2005fa/NNLauthPeople.html
    
  * Cell Phone
     * SMS
     * Google Auth
  * Yubikey
         * https://www.yubico.com/why-yubico/how-yubikey-works/
	 * You should get one
  
     * Zuck Fucked
     * https://www.forbes.com/sites/leemathews/2016/11/16/mark-zuckerberg-hacked-for-the-third-time-this-year/#28a74ee5bd9a
     * Password Resets are scary!
     * Security Questions
        * What is your mother’s maiden name? First dog? Elementary school? All of those things are fairly easy to find online, or just from casual conversation. If someone is trying to steal an account, that will always be the easiest route. Security questions are hard to avoid, but there are easy ways to harden yourself and protect your accounts.
        * - Read this
           * https://www.wired.com/2016/09/time-kill-security-questions-answer-lies/
           * Submit what the article recommends you do
        * Luckily, there is a better way. Instead of forcing you to lie, we are going to introduce you to the ideas of hashing and salting.
       
      * Salting
           * - https://thomashunter.name/blog/password-encryption-hashing-salting-explained/
              * In 2-3 sentences, explain what salting does and why it is important.
           * Combining the ideas of salting and hashing, now learn how you are going to make secure security questions! If we take a hashing algorithm, like MD5, and a unique salt, such as “salty”, we can use the function MD5(_answer_to_question_ + “salty17”). This will create an impossible to guess security question that you can easily use anywhere.
      
# You got tricked!
* You got tricked
	 * You ran someone elses code and gave them access  
	 * You got tricked  https://decentsecurity.com/how-you-get-infected/

	* You ran someone elses code and gave them access
	   * How?	
	   * Phished!!!
	   **Recognize suspicious links and attachments** 		   
                 * https://blog.malwarebytes.com/101/2017/06/somethings-phishy-how-to-detect-phishing-attempts/
		 
		 * Someone just tried to phish me!
                 * https://decentsecurity.com/malware-web-and-phishing-investigation/
             * Report to Academy
                 * **Analyze Phishing for creds email**  
                 * **Malicious attachments**
                 * **Analzye Malicious link**
		    * Set UAC to high
	   * Check for outdated extensions! 
	   * Google scan your computer 
	   * You ran some backdoored shit!
	   
	   Check to see apps youve given access to your email/fb whatever
* Check to see devices with access to your email 
	* Phishing
https://ssd.eff.org/en/module/how-avoid-phishing-attacks
	 * Or you got cred phished (can be done via phone, email, chat, in a form)
* Google oauth worm? Tricked so many people,

# You weren't updated

* Modern systems realize that you are more safe if updates occur automatically. There are very very few situations in which you cannot have auto update turned on. 99% of those situations involve Windows boxes running legacy critical systems. If you don't have auto update turned on... you need to fix that.
* Turn it on for everything
* Android doesnt update well, apple does it very well. 

				 
# OPSEC is king
Someone found you IRL!       
   * OPSEC
     	* What is OPSEC?
	     * Take Uncle Sam's OPSEC
		     * Submit a certificate from the last year
	 * What is the OPSEC Purple Dragon?
	 
	 * Check out the fingerprinter at Panopticlick
	     * https://panopticlick.eff.org/tracker
	        * What does this mean to you?
	 * Got 'em with EXIF data
	    * https://gizmodo.com/5901430/these-breasts-nailed-anonymous-hacker-in-fbi-case
	    * **Get GPS coords from EXIF data**
	 * Compartmentalization
		  * This is very very common. Doesnt need to be technical, just detective work and not being a dumbass.
	       	     * DPR got got.  
		     * Do the OPSEC scavenger hunt
			 * "_name_ "/email/username
			 * Spokeo/and Such
			 * Obituaries
			 * Username reuse site
			 * Internet Archive
			 * Soooo many more
	 * Hacker Opsec with the Grugq
		     * http://blogsofwar.com/hacker-opsec-with-the-grugq/
		 * Identify which of these things you have done
		     * https://gist.github.com/grugq/353b6fc9b094d5700c70
		 * Grugq 10 Commandments
		     * https://grugq.tumblr.com/post/60463307186/rules-of-clandestine-operation
		 * 10 Crack Commandments 
		     * https://www.youtube.com/watch?v=ZYb_8MM1tGQ
		 * 10 Hack Commandments
			https://www.youtube.com/watch?v=Sr8ILq1a_yw


	     * Recommended:
		  * Hacker OPSEC talk 
		     * https://www.youtube.com/watch?v=9XaYdCdwiWU
		  * Dulles' 73 Rules 
		     * http://www.oss.net/dynamaster/file_archive/100102/0a947a77d762061cc87ec541c2d2dcc7/2010-01-02%20Dulles%20on%20Tradecraft%20via%20Srodes.pdf
		 * Moscow Rules  
		     * https://www.spymuseum.org/exhibition-experiences/online-exhibits/argo-exposed/moscow-rules/

  	   * **Use a Burner email**
       * **Burner phone number**
   * **Create a fake person**
               * **Create a fake facebook, twitter, linkedin, ...**

# Hostile Networks
## Intro
Add this to the list of security truisms.

Any network connected to the internet must be considered hostile. Most intranets should be considered hostile to. In fact, it is hard to imagine a more "hostile" network than a DoD network.

But what does "hostile" mean? In this case, the general idea is that if computer A wishes to communicate with computer C, that means that they need to send all of their traffic through computer B. Gentleman's agreements not to look at that traffic might have worked on Arpanet, but not anymore.

From Internet Service Providers (ISPs) working with governments to snoop on all your traffic, to deep sea submarine cable intercepts to sketchy free wifi hotspots, your internet browsing is recorded by a lot of people.

This next section skips over the technical details of network ownage (while giving you plenty to research on your own time), and focuses on the principles that can protect you and specific steps you can take to protect yourself.

Recommended Listening: The Hostile Gospel, Talib Kweli

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


	   
# Someone else got Owned
* Someone else got tricked/hacked
    * Someone else got tricked/hacked
       * Your security is only as good as your weakest link
       * Supply chain attack
       * Home depot hack
          * https://krebsonsecurity.com/2014/02/target-hackers-broke-in-via-hvac-company/
       * RSA Keys
          * That filthy hack
	  * https://bits.blogs.nytimes.com/2011/04/02/the-rsa-hack-how-they-did-it/
       * Bit9 Hack
          * https://krebsonsecurity.com/2013/02/security-firm-bit9-hacked-used-to-spread-malware/
	  
 
			 
SIGN UP for havIbeenpwned

Get SIGNAL
If someone hacks your phone, it doesn't matter
If someone gets someone in your groups phone, it doesnt matter	   

# They got your IP address
https://ssd.eff.org/en/module/how-circumvent-online-censorship

* Someone saw your IP address!!!
   * visiting a website... whats my IP
       * **LOIC**
   * GeoIP
   * proxy
          * We made one for you
      * port forward
      * proxychains! 
   * **IP from pic viewer **
      * https://iplogger.org/
   * **Honeydocs**
      * https://github.com/threatstack/honeyfiles
  	   * Use a VPN
      * We made one for you
     
       * TOR
       * https://danielmiessler.com/study/internet-deep-dark-web	
       
# Physical attacks
* Physical security
	* "Evil Maid"
	    * USB Malware
	       * Stuxnet spread
	       * Rubberducky
	       * BashBunny
	    * if someone has hands on keyboard, they own that computer
	    * "Rubber hose cryptography"
		* https://en.wikipedia.org/wiki/Rubber-hose_cryptanalysis
		* https://xkcd.com/538/
		 
   * Full Disk Encryption
          * OS 
	  * Truecrypt style
	  
	  
   * **Do a linux password reset **
   * **Do a windows stickykeys reset **
  
  * What is BIOS? Why do you encrypt it?

   * Rubber Hose
        * https://www.schneier.com/blog/archives/2009/07/laptop_security.html
	* Truecrypt
	   * https://en.wikipedia.org/wiki/TrueCrypt
	      * plausible deniability
	      * cold boot attack
	     
	     * Black Bag Cryptanalysis
	     https://en.wikipedia.org/wiki/Black-bag_cryptanalysis
	      
	* Legal issues surrounding forced password disclosure
	
	* Biometrics
	   * Fingerprint unlocks
	   * retina/voice/face
	   * Legal stuff
         

		 
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



full disclosure, responsible disclosure,.... selling. 



bug bounty program

hackerone account/bugcrowd account

