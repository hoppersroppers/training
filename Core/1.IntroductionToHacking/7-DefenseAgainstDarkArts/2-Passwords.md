# You used a shitty password 
https://ssd.eff.org/en/module/creating-strong-passwords
 
Passwords are hard, and losing your primary email can pretty much stop your life as you attempt to regain control. Luckily, there is a lot you can do to keep yourself from becoming the low hanging fruit. After this section, not only will you be able to protect yourself, but you’ll be able to share this with others.

Tasks:
* Read this: http://www.passwordanalytics.com/theory/passwords/
* Read Passwords 101 and submit one example each of the three ways you authenticate yourself.
* Read Good Passwords 101 and submit a description of what makes a good password
* Read Strength 101 and submit a description of what makes a strong password
* Read Pass-Phrase and describe how pass phrases balance being a good password and a strong password.
* Read Cracking and explain which technique an attacker would use to attack a password that they knew to be 6 random alpha numeric characters
* Read Cracking and explain which technique an attacker would use to attack a password that they knew to be three random words added together.
* Read this and follow interesting links: https://www.usna.edu/CyberDept/sy110/lec/cryptHashPswd/lec.html
* https://xkcd.com/936/






Here is a brief experiment for you to try. Try to make a rough guess how many web sites you use on a regular basis use your primary email as their account recovery address. Now, try to think about which of those sites are the most important to you that they remain secure; social media, banking, other email accounts. Now think of the sketchy sites you reuse the same password on. If those sketchy sites are breached, and the attacker gets your password, they can try it against your email. If they get your email, they can use it to take your other accounts.

	
### Password Managers

All is not lost however, luckily you do not have to memorize hundreds of high entropy passwords or carry them around in a locked diary. Password managers provide the ability to generate and store secure passwords across devices, all controlled by a single master password. This means you only need to know one password, and the rest can be pseudo-randomly generated. 

Tasks:
* Read this: https://www.howtogeek.com/141500/why-you-should-use-a-password-manager-and-how-to-get-started/
* Submit a 2-3 sentence statement trying to convince my grandma to use a password manager.
* Relevant XKCD https://www.explainxkcd.com/wiki/index.php/936#Explanation
* What password has 2^44 bits of entropy?
* Install LastPass https://lastpass.com/
* Make your password for Lastpass something you have never used before Now that everything will be stored in the same location, you need to protect your lastpass with your life. 
* Make a new gmail account with a good password.
* Setup your Lastpass to be recoverable through this email account only, not your usual account.
* Never use this new email for anything else ever again.
* Complete the LastPass Security challenge
 
### Multi Factor Authentication
  
 Tasks: 
* Read this: https://www.cs.cornell.edu/courses/cs513/2005fa/NNLauthPeople.html
* What is the definition of multi factor auth?
* What does multi factor provide?
* What does it not provide?
* Download GoogleAuth 
* Enable Multifactor on your Lastpass Account. Read through the options https://www.lastpass.com/multifactor-authentication and see what the different varieties are.
* Enable Multifactor on your GitHub
* From a risk perspective, do you really need multifactor on your github?
* Remove multifactor from your Github
* Put multifactor on whatever other accounts you think deserve that level of protection. https://twofactorauth.org/
* Read this: https://www.yubico.com/why-yubico/how-yubikey-works
* You should get a couple.

A brief note: Cell phone text messages are commonly used for multifactor. These are not great, because a) someone can steal your phone number and get the texts sent to them and b) intercept of text messages. However, those things are not in your threat model unless you are famous or have cryptocurrency wallets with sms 2 factor. 

Another note: Just because you have 2 factor doesn't mean you can't get phished for it!
     
### Security Questions and Password Resets

What is your mother’s maiden name? First dog? Elementary school? All of those things are fairly easy to find online, or just from casual conversation. If someone is trying to steal an account, that will always be the easiest route. Security questions are hard to avoid, but there are easy ways to harden yourself and protect your accounts.
 
Tasks: 
* Read this: https://www.wired.com/2016/09/time-kill-security-questions-answer-lies/
* Submit what the article recommends you do

Luckily, there is a better way. Instead of forcing you to lie, we are going to introduce you to the ideas of hashing and salting.

### Hashing and Salting

Tasks:
* Read this: https://crackstation.net/hashing-security.htm. Not all of it, unless you really want to, just enough to answer these questions.
* In 2-3 sentences explain hashing and why it is important
* Describe each of the ways passwords are cracked
* In 2-3 sentences, explain what salting does and why it is important.

Combining the ideas of salting and hashing, now learn how you are going to make secure security questions! First, as a rule, don't use uppercase letters, spaces, or punctuation ever in your security questions. Why? Nothing about security, it just makes them easier to remember. Then if we take a hashing algorithm, like MD5, and a unique salt, such as “salty17”, we can use the function MD5(_answer_to_question_ + “salty17”). This will create a very very hard to figure out security question that you can easily use anywhere. 

Or, if you are on a computer with your password manager, just write that shit down in your secure notes for a site. If they get your lastpass account you are screwed anyway, so don't worry about it.

# L0phtcrack tangent
* http://www.washingtonpost.com/sf/business/2015/06/22/net-of-insecurity-part-3/?utm_term=.ea6927af0bd7
* en.wikipedia.org/wiki/L0pht
* Responsible Hacking

# You Got Phished For Your Password

You can always get tricked with a good email or malicious link that leads you to a login page. Always, always, always, always look at the full URL. Green locks and any other bells and whistles won't help you. There is always a small chance that your DNS is being hijacked and the URL is right, in which case your browser will tell you that the HTTPS key has changed. Long story short, use chrome, listen to your browser and think. It's happened to me, it might happen to you, just don't lose your email or password manager. 

There is more information on this you have already gotten. 

# Someone else got popped

Tasks:
* Read this: https://haveibeenpwned.com/FAQs
* Sign up for haveIbeenpwned with all of your emails, especially older ones

# Default Passwords

There are a lot of default passwords out there in the world. You can use them to get free wifi, but the bad guys can use them too. 

Routers, Internet of Things devices, and web applications are common victims of default passwords. 
If you have the ability to change the password, change the password. If you don't change the defaults, you are begging to get added to a botnet, or worse. 



  
  
