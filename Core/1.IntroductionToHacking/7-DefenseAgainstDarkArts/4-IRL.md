# OPSEC is King

If someone has found you in real life, the game is usually over. There are all sorts of great technical approaches to protecting yourself we have gone over already, but technology only goes so far. There is always a log created digitally and if a motivated attacker wants you, they will get you technically. OPSEC is what keeps you off the radar, and if you are going to be on the radar, gives them a cold trail and a fake account to chase into the ground. If you follow these rules, you will do much better towards not getting arrested.

## What is OPSEC?

Tasks:

1. Submit what is the OPSEC Purple Dragon
2. Check out the fingerprinter at Panopticlick: [https://panopticlick.eff.org/tracker](https://panopticlick.eff.org/tracker)
3. Read this: [https://gizmodo.com/5901430/these-breasts-nailed-anonymous-hacker-in-fbi-case](https://gizmodo.com/5901430/these-breasts-nailed-anonymous-hacker-in-fbi-case)
4. Give me the GPS coords for this picture: [https://exposingtheinvisible.org/ckeditor_assets/pictures/32/content_example_ibiza.jpg](https://exposingtheinvisible.org/ckeditor_assets/pictures/32/content_example_ibiza.jpg) . I recommend this site: [http://exif.regex.info/](http://exif.regex.info/)

## Compartmentalization

Tasks:
* Listen to the 10 Crack Commandments: <https://www.youtube.com/watch?v=ZYb_8MM1tGQ>
* Read this: <https://medium.com/@thegrugq/operational-security-and-the-real-world-3c07e7eeb2e8>
1. Submit the reasoning behind compartmentalization and how it fits into your risk model?
* Read This: <https://blogsofwar.com/hacker-opsec-with-the-grugq/>
* Read this: <https://gist.github.com/grugq/353b6fc9b094d5700c70>
1. Identify which of these things you have not done yet and do them.
* Read Grugq's Commandments: <https://grugq.tumblr.com/post/60463307186/rules-of-clandestine-operation>. The Grugq, who you might remember from the article about zero day brokers, is a famous hacker who is most known recently for his OPSEC and high level work. He is an absolute Twitter must follow and you can basically take anything he says as infosec gospel.

* Listen to the 10 Hack Commandments: <https://www.youtube.com/watch?v=Sr8ILq1a_yw>. It's by a guy called Dual Core, makes some pretty dope stuff for a rapper who writes for nerds. His number one song is 'Drink All the Booze, Hack All the Things' <https://www.youtube.com/watch?v=FoUWHfh733Y>. Let's put it this way, hackers don't take themselves all that seriously, and they can do some pretty cringey shit. If you listen to the lyrics to 'Hack All the Things' you will probably understand about one third of the references, at best. If you don't like it or are too cool for nerdcore rap, that's fine. If you stick around eventually you'll understand most of it and you'll go nuts when someone throws it on during a late night hack sesh after you've been passing around a bottle of whiskey. Hackerdoms not so great relationship with alcohol and cringey shit aside, it all comes with the culture.

If you have the time, these are all highly recommended, if not, add them to your 'Read At Some Point' tab in the Learning Sheet:
* Hacker OPSEC talk: <https://www.youtube.com/watch?v=9XaYdCdwiWU>
* Dulles' 73 Rules: <https://www.oss.net/dynamaster/file_archive/100102/0a947a77d762061cc87ec541c2d2dcc7/2010-01-02%20Dulles%20on%20Tradecraft%20via%20Srodes.pdf>
* Moscow Rules: <https://en.wikipedia.org/wiki/The_Moscow_rules>


# Physical attacks

A physical attack on your computer, called an "Evil Maid", is a classic attack and near impossible to defeat. If someone has hands on keyboard after stealing your device, they own that computer unless you have protected it properly. If you have protected it properly and someone modifies the hardware, then you use it, then you are still screwed. If someone has you and the computer, you are screwed. Long story short, it is better for them to not know you are worth attacking, thus, OPSEC. However, sometimes you can't do that. Maybe you are a high profile individual who is in a hotel, maybe you live in a government dorm, maybe you are traveling and get border searched. This is the guide for those times.

Tasks:

* Read this: <http://images.secure.f-secure.com/Web/FSecure/%7B319382b2-a040-4c88-bd94-20eed01bf22f%7D_F-Secure-Evil-Maid-Guide.pdf>
* Where does an evil maid attack fall into your personal threat model?

You can also mount an encrypted partition in your OS, and use that to hold a virtual machine to do your important work on. That gives you a ton of deniability, especially with the ability to make multiple partitions that unlock to different passwords. Remember though, if you get hacked on the outside, you get hacked in the VM as well. Either way, you need FDE and secure boot if you want to beat an evil maid.

Alright, now that you know that you need FDE and Secure Boot if Evil Maid attacks fit your threat model, lets go into various physical attacks on a computer and defenses against them.

1. Tackling you off of the computer while logged in
  * This is how the Dread Pirate Roberts, the admin of the Silk Road, aka the best place to buy drugs in history, was arrested.
    * <https://arstechnica.com/tech-policy/2013/10/how-the-feds-took-down-the-dread-pirate-roberts/>
        * You can try a quick shutdown, there are various tools that connect to bracelets which, if you are tackled away from your computer, can automatically shut it down.
	* But even if you get the computer shut down, that doesn't mean they LE can't recover encryption keys from it if they are prepared. While this sounds hard, I've done one before in a controlled environment. Actually pretty easy.
	    * <https://en.wikipedia.org/wiki/Cold_boot_attack>
      1. Understanding a cold boot attack requires an understanding of electricity and how RAM stores DATA. Write about how it is possible.


2. Breaking in to your hotel room and installing a keylogger, then breaking back in later and stealing your laptop now that they have the password.
        * All of the next few ways fall under something referred to as black bag cryptanalysis. <https://en.wikipedia.org/wiki/Black-bag_cryptanalysis>

        Tasks:
        These tasks are not only illustrative of threats to you, but at some point you will be locked out of your shit and need to get back in. This is how you will do it. There are ways to ensure this doesn't work, but does that fit your threat model? Didn't think so. These tasks are fairly complicated but there are many resources online how to do them. Follow the tutorials closely (make sure it is a recent tutorial), and you can't mess anything up too badly.

        1. Do a Linux password reset on your VM using the GRUB bootloader attack. This will be the same for the vast majority of Linux VMs, but a general rule is that you can just Google how to do it for the VM you are on. This one is generally known as a Grub Bootloader attack. Here is a starting point. <https://itsfoss.com/how-to-hack-ubuntu-password/> Write a couple sentences about what you learned from this.

        2. Do a Windows stickykeys reset on your actual computer. This literally works on every single version of Windows, and every Windows computer you have ever been on. This one is generally known as the stickykeys or "sethc" reset. You'll figure out why that is. Here is a starting point. <https://www.top-password.com/blog/reset-windows-10-password-with-sticky-keys/>. One interesting note is that you might have to boot into safe mode for the stickykeys login as Windows Defender does interesting things. This link will bring you to the actual way to do this. <https://www.top-password.com/knowledge/reset-windows-10-password.html>

Write a couple sentences about what you learned from this.

3. Malicious hardware connected to a turned on computer
There are many many types of malicious hardware that can be connected to a live computer and take it over. These are some examples. While they all are under brand names, they are representative of entire families of malicious USB devices. I wouldn't recommend buying any of them, just make your own. There are open source versions of all of them. Except for the OMG Cable. You can't build that capability yourself.
  * Hey, this is how Stuxnet worked! <https://arstechnica.com/tech-policy/2011/07/how-digital-detectives-deciphered-stuxnet-the-most-menacing-malware-in-history/>
	* USB Malware
	       * Badusb <https://arstechnica.com/information-technology/2014/07/this-thumbdrive-hacks-computers-badusb-exploit-makes-devices-turn-evil/>
	       * Rubberducky <https://shop.hak5.org/products/usb-rubber-ducky-deluxe>
	       * BashBunny <https://shop.hak5.org/collections/physical-access/products/bash-bunny>
         * OMG Cable <https://www.bleepingcomputer.com/news/security/new-offensive-usb-cable-allows-remote-attacks-over-wifi/>

  1. How did the Stuxnet USB attack work?
  2. How does the BadUSB attack work?
  3. How does the RubberDucky attack work?
  4. How does the BashBunny attack work?
  5. How does the OMG Cable attack work?

	* The best defense is to turn off your computer when you leave and have a protected BIOS.

4. Pre-Installed Hardware Attacks
	* Hardware intercepts
	  	* Some chips will get intercepted en route, replaced/modified, and sent to their final destination
	* Backdoored Chips
		* Some chips will come off the assembly line with backdoors in them already. Not many of them... but it can and probably has happened.
    * <https://en.wikipedia.org/wiki/Hardware_backdoor>


5. Electronic Emissions
        * Read this: <https://en.wikipedia.org/wiki/Van_Eck_phreaking>

6. Taking you and your computer and forcing you to give up password
This can take the form of a lengthy interrogation and a court battle, or getting tortured. Either way. You're in a world of hurt if this is what it comes down to.

  * "Rubber hose cryptography"
		* <https://en.wikipedia.org/wiki/Rubber-hose_cryptanalysis>
		* <https://xkcd.com/538/>
        * Some encryption tools allow the possibility of multiple partitions, so that multiple passwords can be used. Only one password unlocks what you are actually trying to hide, others open different partitions, and there is no way of proving that there are multiple partition/password pairs... this doesn't work very well legally, but might work. A little bit.
	    * Legal issues surrounding forced password disclosure
              * There is more constitutional law in this field than you ever expected. Further on courses will discuss how all this plays together but:
        	      * Basically, US you are good, plead the 5th, self-incrimination. You'll still probably go down, but not for what is on the hard drive.
        	      * Europe, you are going to jail
        	      * Most other Western countries, jail
        	      * "Not chill" countries, beaten until you give it up, then jail

	* Biometrics
	   * If your device unlocks with anything on your body, they can just take you and open your stuff.
	   * Fingerprint/retina/voice/face unlocks are not protected by US Constitution, they can just make you unlock these things if they have you.

# Lockpicking
Lockpicking and other security bypass techniques are very popular in the community, for obvious reasons. Many conferences have lockpick competitions and plenty of people carry picks around, because there is nothing worse than getting locked out of things you are allowed access to, but don't have a key.

Read this: <https://www.art-of-lockpicking.com/how-to-pick-a-lock-guide/>.

At some point we will figure out getting lockpicks to participants so that they can practice.


# Things to Potentially Add

### Opsec Scavenger Hunt Do the OPSEC scavenger hunt
* "_name_ "/email/username
* Spokeo/and Such
* Obituaries
* Username reuse site
* Internet Archive	  

### Securing your Life

Tasks:
* Look at this: <https://privacy.com/>
* Create a fake person
   * Get a burner email
   * Get a burner phone number
   * fake facebook
   * twitter
   * linkedin
