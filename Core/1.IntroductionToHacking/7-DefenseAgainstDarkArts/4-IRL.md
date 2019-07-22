# OPSEC is king

If someone has found you in real life, the game is over. There are all sorts of great technical approaches to protecting yourself we have gone over already, but technology only goes so far. There is always a log created digitally and if a motivated attacker wants you, they will get you technically. OPSEC is what keeps you off the radar, and if you are going to be on the radar, gives them a cold trail and a fake account to chase into the ground. If you follow these rules, you will do much better towards not getting arrested. 

## What is OPSEC?

Tasks:

1. Submit what is the OPSEC Purple Dragon
2. Check out the fingerprinter at Panopticlick: [https://panopticlick.eff.org/tracker](https://panopticlick.eff.org/tracker)
3. Read this: [https://gizmodo.com/5901430/these-breasts-nailed-anonymous-hacker-in-fbi-case](https://gizmodo.com/5901430/these-breasts-nailed-anonymous-hacker-in-fbi-case)
4. Give me the GPS coords for this picture: [https://exposingtheinvisible.org/ckeditor_assets/pictures/32/content_example_ibiza.jpg](https://exposingtheinvisible.org/ckeditor_assets/pictures/32/content_example_ibiza.jpg) . I recommend this site: [http://exif.regex.info/](http://exif.regex.info/)

## Compartmentalization


Tasks:
* Listen to the 10 Crack Commandments: https://www.youtube.com/watch?v=ZYb_8MM1tGQ 
* Read this: https://medium.com/@thegrugq/operational-security-and-the-real-world-3c07e7eeb2e8
* Submit the reasoning behind compartmentalization and how it fits into your risk model?
* Read This: http://blogsofwar.com/hacker-opsec-with-the-grugq/
* Read this: https://gist.github.com/grugq/353b6fc9b094d5700c70 
* Identify which of these things you have not done yet and do them.
* Read Grugq's Commandments: https://grugq.tumblr.com/post/60463307186/rules-of-clandestine-operation

* Listen to the 10 Hack Commandments: https://www.youtube.com/watch?v=Sr8ILq1a_yw. It's by a guy called Dual Core, makes some pretty dope stuff for a rapper who writes for nerds. His number one song is 'Drink All the Booze, Hack All the Things' https://www.youtube.com/watch?v=FoUWHfh733Y. Let's put it this way, hackers don't take themselves all that seriously, and they can do some pretty cringey shit. If you listen to the lyrics to 'Hack All the Things' you will probably understand about one third of the references, at best. If you don't like it or are too cool for nerdcore rap, that's fine. If you stick around eventually you'll understand most of it and you'll go nuts when someone throws it on during a late night hack sesh after you've been passing around a bottle of whiskey.

If you have the time, these are all highly recommended, if not, add them to your 'Read At Some Point' tab in the Learning Sheet:
* Hacker OPSEC talk: https://www.youtube.com/watch?v=9XaYdCdwiWU
* Dulles' 73 Rules: http://www.oss.net/dynamaster/file_archive/100102/0a947a77d762061cc87ec541c2d2dcc7/2010-01-02%20Dulles%20on%20Tradecraft%20via%20Srodes.pdf
* Moscow Rules: https://en.wikipedia.org/wiki/The_Moscow_rules

### Opsec Scavenger Hunt Do the OPSEC scavenger hunt
* "_name_ "/email/username
* Spokeo/and Such
* Obituaries
* Username reuse site
* Internet Archive	  
		  
# Securing your Life

Tasks: 
* Look at this: https://privacy.com/
* Create a fake person
   * Get a burner email 
   * Get a burner phone number
   * fake facebook
   * twitter 
   * linkedin
	      
# Physical attacks

A physical attack on your computer, called an "Evil Maid", is a classic attack and near impossible to defeat. If someone has hands on keyboard after stealing your device, they own that computer unless you have protected it properly. If you have protected it properly and someone modifies the hardware, then you use it, then you are still screwed. If someone has you and the computer, you are screwed. Long story short, it is better for them to not know you are worth attacking, thus, OPSEC. However, sometimes you can't do that. Maybe you are a high profile individual who is in a hotel, maybe you live in a government dorm, maybe you are traveling and get border searched. This is the guide for those times. 

Tasks:
* Read this: http://images.secure.f-secure.com/Web/FSecure/%7B319382b2-a040-4c88-bd94-20eed01bf22f%7D_F-Secure-Evil-Maid-Guide.pdf
* Where does an evil maid attack fall into your personal threat model?

You can also mount an encrypted partition in your OS, and use that to hold a virtual machine to do your important work on. That gives you a ton of deniability, especially with the ability to make multiple partitions that unlock to different passwords. Remember though, if you get hacked on the outside, you get hacked in the VM as well. Either way, you need FDE and secure boot if you want to beat an evil maid.

Alright, now that you know that you need FDE and Secure Boot, lets go into various physical attacks on a computer and defenses against them.

1. Tackling you off of the computer while logged in
        * You can try a quick shutdown
	* Read about Cold Boot attacks
	    * https://en.wikipedia.org/wiki/Cold_boot_attack
	    * While this sounds hard, I've done one before in a controlled environment. Actually pretty easy.
	    
2. Breaking in to your hotel room and installing a keylogger, then breaking back in later and stealing your laptop now that they have the password. Or just arresting you.
        * https://en.wikipedia.org/wiki/Black-bag_cryptanalysis
	* Classic Boot attack
	* Installing keylogger
	
3. Malicious hardware to a turned on computer
	* USB Malware
	       * BAdusb
	       * Rubberducky
	       * BashBunny
	* FIREWIRE
	* Turn off your computer when you leave 
	
4. User Introduced Attacks
	* Hardware intercepts
	  	* Some chips will get intercepted en route, replaced/modified, and sent to their final destination
	* Backdoored chips
		* Some chips will come off the assembly line with backdoors in them already

4. Malicious hardware to turned off compter
        * Throw a new chip on your computer
	* Keylogger in keyboard
	* NSA Playset: http://www.nsaplayset.org/chuckwagon
	
4. Electronic Emissions
        * Read this: https://en.wikipedia.org/wiki/Van_Eck_phreaking
	
5. Taking you and your computer and forcing you to give up password
	* "Rubber hose cryptography"
		* https://en.wikipedia.org/wiki/Rubber-hose_cryptanalysis
		* https://xkcd.com/538/
        * Some encryption tools allow the possibility of multiple partitions, so that multiple passwords can be used. Only one password unlocks what you are actually trying to hide, others open different partitions, and there is no way of proving that there are multiple partition/password pairs... this doesn't work very well legally, but might work. A little bit. 
	    * Legal issues surrounding forced password disclosure
	      * Basically, US you are good, plead the 5th, self-incrimination. 
	      * Europe, you are going to jail
	      * Most other countries, jail
	      * Not fun countries, beaten until you give it up
	      
	* Biometrics
	   * If your device unlocks with anything on your body, they can just take you and open your stuff. 
	   * Fingerprint/retina/voice/face unlocks are not protected by Constitution, they can just make you unlock these things if they have you. 
	   
Tasks:
* Do a linux password reset on your VM
* Do a windows stickykeys reset on your actual computer
* https://securityonline.info/evilabigail-automated-linux-evil-maid-attack/
  
	
         
