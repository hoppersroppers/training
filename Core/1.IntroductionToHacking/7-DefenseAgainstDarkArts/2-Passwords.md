# You used a shitty password
<https://ssd.eff.org/en/module/creating-strong-passwords>

Passwords are hard, and losing your primary email can pretty much stop your life as you attempt to regain control. Luckily, there is a lot you can do to keep yourself from becoming the low hanging fruit. After this section, not only will you be able to protect yourself, but you’ll be able to share this with others.

Tasks:
1. Read this: <https://www.passwordanalytics.com/theory/passwords/>
2. Read Passwords 101 and submit one example each of the three ways you authenticate yourself.
3. Read Good Passwords 101 and submit a description of what makes a good password
4. Read Strength 101 and submit a description of what makes a strong password
5. Read Pass-Phrase and describe how pass phrases balance being a good password and a strong password.
6. Read Cracking and explain which technique an attacker would use to attack a password that they knew to be 6 random alpha numeric characters
7. Read Cracking and explain which technique an attacker would use to attack a password that they knew to be three random words added together.
8. Read this and follow interesting links: <https://www.usna.edu/CyberDept/sy110/lec/cryptHashPswd/lec.html>
9. <https://xkcd.com/936/>

Here is a brief experiment for you to try. Try to make a rough guess how many web sites you use on a regular basis use your primary email as their account recovery address. Now, try to think about which of those sites are the most important to you that they remain secure; social media, banking, other email accounts. Now think of the sketchy sites you reuse the same password on. If those sketchy sites are breached, and the attacker gets your password, they can try it against your email. If they get your email, they can use it to take your other accounts.


### Password Managers

All is not lost however, luckily you do not have to memorize hundreds of high entropy passwords or carry them around in a locked diary. Password managers provide the ability to generate and store secure passwords across devices, all controlled by a single master password. This means you only need to know one password, and the rest can be pseudo-randomly generated.

Tasks:
1. Read this: <https://www.howtogeek.com/141500/why-you-should-use-a-password-manager-and-how-to-get-started/>
2. Submit a 2-3 sentence statement trying to convince my grandma to use a password manager.
3. Relevant XKCD <https://www.explainxkcd.com/wiki/index.php/936#Explanation>. What password has 2^44 bits of entropy?
4. Install LastPass https://lastpass.com/
5. Make your password for Lastpass something you have never used before. Now that everything will be stored in the same location, you need to protect your lastpass. Write this password down in a variety of places that you will not lose. Or just remember it. I recommend writing it down.
6. Make a new gmail account with a good password.
7. Setup your Lastpass to be recoverable through this email account only, not your usual account.
8. Never use this new email for anything else ever again other than
9. Complete the LastPass Security challenge

### Multi Factor Authentication


Tasks:
1. Read this: <https://www.cs.cornell.edu/courses/cs513/2005fa/NNLauthPeople.html>
2. What is the definition of multi factor auth?
3. What does multi factor provide?
4. What does it not provide?
5. Download GoogleAuth
6. Enable Multifactor on your Lastpass Account. Read through the options <https://www.lastpass.com/multifactor-authentication> and see what the different varieties are.
7. Enable Multifactor on your GitHub
8. From a risk perspective, do you really need multifactor on your github?
9. Remove multifactor from your Github
10. Put multifactor on whatever other accounts you think deserve that level of protection. <https://twofactorauth.org/>
11. Read this: <https://www.yubico.com/why-yubico/how-yubikey-works>

You could probably get a couple, and then set it up with <https://landing.google.com/advancedprotection/>. Or not. You probably don't need it. My philosophy is I can't properly tell people to do things for their security if I don't do it myself and understand the pain points.

A brief note: Cell phone text messagesaka SMS are commonly used for multifactor auth. These are not great, because
a) someone can steal your phone number and get the texts sent to them  (https://www.wired.com/story/sim-swap-attack-defend-phone/)
b) intercept of text messages (https://www.theguardian.com/technology/2016/apr/19/ss7-hack-explained-mobile-phone-vulnerability-snooping-texts-calls)

However, those things are not in your threat model unless you are famous or have cryptocurrency wallets.

Another note: Just because you have 2 factor doesn't mean you can't get phished for it!

### Security Questions and Password Resets

What is your mother’s maiden name? First dog? Elementary school? All of those things are fairly easy to find online, or just from casual conversation. If someone is trying to steal an account, that will always be the easiest route. Security questions are hard to avoid, but there are easy ways to harden yourself and protect your accounts.

Tasks:
* Read this: <https://www.wired.com/2016/09/time-kill-security-questions-answer-lies/>
* Submit what the article recommends you do

Luckily, there is a better way. Instead of forcing you to lie, we are going to introduce you to the ideas of hashing and salting.

### Hashing and Salting

Tasks:
* Read this: <https://crackstation.net/hashing-security.htm>. Not all of it, unless you really want to, just enough to answer these questions.
* In 2-3 sentences explain hashing and why it is important
* Describe each of the ways passwords are cracked
* In 2-3 sentences, explain what salting does and why it is important.

Combining the ideas of salting and hashing, now learn how you are going to make secure security questions! First, as a rule, don't use uppercase letters, spaces, or punctuation ever in your security questions. Why? Nothing about security, it just makes them easier to remember. Then if we take a hashing algorithm, like MD5, and a unique salt, such as “salty17”, we can use the function MD5(_answer_to_question_ + “salty17”). This will create a very very hard to figure out security question that you can easily use anywhere.

Or, if you are on a computer with your password manager, just write that shit down in your secure notes for a site. If they get your lastpass account you are screwed anyway, so don't worry about it.

# L0phtcrack tangent
* <http://www.washingtonpost.com/sf/business/2015/06/22/net-of-insecurity-part-3/?utm_term=.ea6927af0bd7>
* en.wikipedia.org/wiki/L0pht
* Responsible Hacking

# You Got Phished For Your Password

You can always get tricked with a good email or malicious link that leads you to a login page. Always, always, always, always look at the full URL. Green locks and any other bells and whistles won't help you. But.... there is always a small chance that your DNS is being hijacked and the URL is right, in which case your browser will tell you that the HTTPS key has changed. Long story short, use chrome, listen to your browser and think. It's happened to me, it might happen to you, just don't lose your email account, or your password manager.

There is more information on this you have already gotten.

# Someone else got popped

Tasks:
* Read this: <https://haveibeenpwned.com/FAQs>
* Sign up for haveIbeenpwned with all of your emails, especially older ones

# Default Passwords

There are a lot of default passwords out there in the world. You can use them to get free wifi, but the bad guys can use them too.

Routers, Internet of Things devices, and web applications are common victims of default passwords.
If you have the ability to change the password, change the password. If you don't change the defaults, you are begging to get added to a botnet, or worse.

If you ever install an application and it has a default password, changwe that shit.
