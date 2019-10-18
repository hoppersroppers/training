# Cyber Killchain
So how has security adapted to face all these threats? Basically, the most modern idea is the idea of defense in depth, making it so the bad guys have to beat layer after layer of security in order to get in, and then back out. The go-to model is the cyber killchain by Lockheed Martin, and while it gets a ton of crap, it is honestly a very good way of looking at it.

Read this: www.lockheedmartin.com/content/dam/lockheed/data/corporate/documents/LM-White-Paper-Intel-Driven-Defense.pdf

Make sure you know the different layers of the killchain.
Write a sentence describing each and provide three examples. If you can't think of examples, google for em. Don't worry too much about being right.

1. Recon
2. Weaponization
3. Delivery
4. Exploitation
5. Installation
6. Command and Control
7. Actions on Objectives

One of the most common arguments against the killchain is that "Actions on Objectives" is too vague. For one, all of the other steps of the killchain can occur as an action on objective if the attacker uses it to attack something else, which is known as pivoting. But there are many other "post-exploitation" objectives of an attacker, which range from installing backdoors to bricking the device.

There are 5 P's of Post-Exploitation:

* Persistence = Find a way to maintain access
* Privilege Escalation = Find a way to get a higher level of access than you already have
* Pilfer = Steal things
* Pillage = Break things.
* Pivot = Move from one box to another and start the killchain all over again.

I will write a good post on this at some point, but for now, just try to remember what each of those things means.

Task:

Describe a hypothetical attack on a user via email, using your current understanding, from recon all the way through all the post exploitation possibilities. It is fine if you don't have the technical understanding, we are just trying to make sure you have the concepts down. You are going to look back at this scenario later in the course and do it again, once you have more technical concepts down.

# Pyramid of Pain

So now we are able to identify specific actions, now it is time to break down how to make it hard for the attacker. Knowing the attacker's TTPs, is hard to do, and you really can't do attribution to a specific actor just using those. This is a good mental model of all the ways you can make it hard for the adversary, as well as identify who they might be.

Read this: <http://detect-respond.blogspot.com/2013/03/the-pyramid-of-pain.html>

Tasks:
1. For each level of the pyramid of pain, describe it in your own words, and provide the primary strength and weakness of each.
2. You might realize that tools and the first T in TTPs (Tools) are both on there. The primary difference is that tools is removing the adversary's ability to use a tool, while Tools is identifying the behavior caused by various tools that accomplish the same thing. Write a few sentences on what behavioral detection means and how it could work in some fancy startup.
3. Write a few sentences on how you could use the items in the pyramid of pain to identify a threat group.

# Diamond Model

Alright, so now we are able to identify a specific actor's general profile and have made ourselves hardened targets. Now, how do we make correlations across various boxes, networks, and organizations? One helpful model for this is the Diamond Model.

Read this: <https://digital-forensics.sans.org/summit-archives/cti_summit2014/The_Diamond_Model_for_Intrusion_Analysis_A_Primer_Andy_Pendergast.pdf>

Tasks:
1. For each corner of the diamond, write a few sentences on what they are.
2. Write a few sentences on how correlation between breaches can be done using the Killchain and the Diamond Model.
3. What is a threat group/activity group? (You may need Google)
4. Write a few sentences on how you can use these pieces of information to build an identity for an activity group.
5. Write about what the benefits are of creating a named threat/activity group

# Advanced Persistent Threats

I will write something better eventually, but for now, this has most of the information you need.

Read this: <https://www.secureworks.com/blog/advanced-persistent-threats-apt-a>

# APT 1 aka Unit 61398

You may have heard of other Advanced Persistent Threats (APT) by now, but here is the report that got it all started. It was the first report that publically named and provided TTPs and Indicators of Compromise (IOC), as well as identities of a threat group. Now everyone does it, but this is what got the ball rolling in threat intelligence.

Read this: <https://www.fireeye.com/content/dam/fireeye-www/services/pdfs/mandiant-apt1-report.pdf>
