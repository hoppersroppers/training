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
      
 # You Got Phished For Your Password
 
 
   # Default Passwords
   
   On your boxen, IOT, server setups, KALI
   
  # No Password
  
  Way more shit has no password than expected
  
  # Easy Password Resets
  
  
