# Architecture

This is a very short section that we will make longer in the future, but for now, it'll do.

Task: 

For each of these items, define what they are and how they relate to security.

* Modem
* Router
* Switch
* Firewall
* DMZ
* Proxy
* Endpoint/Host
* Server
* Web Application
* Domain Controller

# Domains of Attack
There are a lot of ways for you to get hacked, so there is no way we can go over them all. 

But, we can go over good ways to think about this. 

This site goes over where all your vulnerabilities lie.

https://capec.mitre.org/data/definitions/3000.html

* Social Engineering
* Supply Chain
* Communications
* Software
* Physical Security
* Hardware

Tasks: 

1. For each of the domains of attack, describe in a few sentences what they are and how you can be attacked through them.
2. Describe what "attack surface" means to you.
3. Describe how you would minimize attack surface.

# Attack Mechanisms


Now we can think about how you get attacked in those domains in terms of attack mechanisms as seen here. This is a crazy useful resource that will require its own section someday.

List of Attack Mechanisms:

* Collect and Analyze Information 
* Inject Unexpected Items 
* Engage in Deceptive Interactions 
* Manipulate Timing and State
* Abuse Existing Functionality
* Employ Probabilistic Techniques 
* Subvert Access Control 
* Manipulate Data Structures 
* Manipulate System Resources 

Task: 

For each attack mechanism, describe in two sentences what the thing being attacked is and how they generally work. This is going to take some research, but shouldn't take all that long. You can click to expand to learn more about each type of attack. 

# Attack Methods

Building off of domains of attack, and mechanisms of attack, MITRE also created an unbelievable resource that provides a way of looking at how those mechanisms are applied to the various domains of attack. Unsurprisingly, it is called ATT&CK (Adversarial Tactics, Techniques, and Common Knowledge). This is the real world, practical application of these theories and it lists out the many many many ways that bad guys get in. 

https://attack.mitre.org/wiki/Main_Page

This resource will take a prohibitively long time to go through, and honestly deserves its own course. But if you don't know what each of the items described in it means, you will be hurting in the long term.

We are going to have you read through all of this to help your brain understand what is possible. Consider it a crash course in evil.

Tasks:

1. For the items in Initial Access, write one sentence summarizing how the attack works. 
2. Execution has a lot of complicated things that do not require understanding yet. For now, just write one sentence for the following items:
* Exploitation for Client Execution
* Service Execution
* User Execution
* Script Execution (this is not it's own specific item, but you'll be able to figure it out)
* Operating System Execution (this isn't either)

3. Read through Persistence, but don't worry about understanding most of it. There's a lot of useful technical things in there, but this will help you see words and just familiarize yourself with it.
4. Same with Privilege Escalation, Defense Evasion, Credential Access, Discovery, Lateral Movement, Collection, Exfiltration, Command and Control.... this requires more work... but really just read it and ignore the things that don't make sense. It's good practice. 

Skip Pre-Attack for now. (https://attack.mitre.org/pre-attack/index.php/Main_Page) It requires its own stuff, lot of work to do.

# Penetration Testing

Pen Test is short for penetration testing, which basically means breaking into someone's stuff in order to help make them more secure by identifying vulnerabilities and helping to fix them. In the civilian world, you can do this for a job. While the military has "red teams" which perform attacks on friendly networks to help make our defenses better, the rest of the military who does this kind of work usually doesn't tell the people they hack how to make their systems more secure....Mostly because those people have already been hit in the head with a hellfire missile or shot in the head by a SEAL. But I digress.

On the second page of this cool poster, learn about a sample network pen test.

Read this: https://www.sans.org/security-resources/posters/pen-test-attack-surfaces-tools-techniques/70/download

For anything you do not understand, look it up. If looking up doesn't explain that specific item well in >5 minutes, add your question to your question list and write it at the bottom of your submission.

Task:

In your own words, describe what happened. Don't worry about getting it wrong for now, we'll teach you how to do this eventually. In addition, write out whatever questions you have about this and we'll answer them.

You will be doing this for a few more scenarios, the point of writing out how this happened is so we can help you if you misunderstand things, as well as answer your questions.

# Advanced Pen Test
On the second page of the same poster, learn about an advanced network pen test.

Read this: https://www.sans.org/security-resources/posters/pen-test-attack-surfaces-tools-techniques/70/download

For anything you do not understand, look it up, and if that doesn't work, write it down.

Task:

In your own words, describe what happened so that your grandpa can understand it. You'll learn how to do this too... probably not with a zero day though ;)

In addition, ask questions!!!

# Wireless Pen Test
Same cool poster, learn about a sample wireless pen test.

Read this: https://www.sans.org/security-resources/posters/pen-test-attack-surfaces-tools-techniques/70/download

For anything you do not understand, look it up.

Task:

In your own words, describe what happened so your roomate understands it. We'll do this eventually.

Ask questions as well!!

# Web Application Pen Test

Same poster, learn about a sample web app pen test. 

Read this: https://www.sans.org/security-resources/posters/pen-test-attack-surfaces-tools-techniques/70/download

For anything you do not understand, look it up. Then include it in your description.

Task:

In your own words, describe what happened so the Supe can understand. This one is hard, but fun.

Again, ask questions!

