# Site Introduction
## Why Security?

Computer security is the shield of the modern age. Without the constant battle on the frontlines between the people who want to see technology used for good and the people who want to use it for their own gain, or worse, to limit the rights and freedoms of others, the progress that occurs in the real world because of technology would be dramatically slowed. Security allows trust in technology, which leads to adoption, which leads to progress in one direction, or another. The more people able to help out with that fight, the faster we can move as a society, and less things will get broken and less people will be hurt on the way. That’s why this site exists, and hopefully, if you’re here for the right reasons, you’ll be able to jump into the fight with the tools you need to succeed.

This course is meant to give you, someone new to the security field, and information technology in general, the skills and more importantly, the mindset required to be successful in this line of work. The only way to be good at anything in this field is to become comfortable looking at problems you have never seen before and then finding a way to solve what you are up against. This curriculum is not meant to turn you into a guru, but rather it is to provide you with a solid base of knowledge and mental models relating to security, as well as build your comfort level installing new programs, following tutorials for things you have never heard of before, and using the Linux operating system. If you leave this course with nothing other than an understanding of the hacker mentality, I have been successful by some measure. However, my goal is to help guide you through the first few steps of your journey into this world and to help you find your path afterwards as you develop even more advanced skills and continue your constant growth.

While I have tried to do everything in my ability to make this course self-guided, there are hundreds of places where a questioning attitude will identify clear shortfalls in the content. Some of these are intentional, most of them are not. Your questions and feedback will guide the development of this course so that it can become the best resource possible.

Surrounding this site is a community to help you and provide guidance as you move along.  This community grows with each student who signs up, and our mentors will be there every step of the way to answer questions, explain difficult concepts, and talk about just about anything to help you along the way. Make sure to take full advantage of the many ways we provide to message other mentors so that we can all be part of this together.

# Lessons From Grace Hopper
## Introduction
Our team has gone by many names, but one of our favorite's is Hopper's Roppers. You may have heard of Grace Hopper before because the Cyber Center is going to be named after her.

Images:

![alt text](https://upload.wikimedia.org/wikipedia/commons/a/ad/Commodore_Grace_M._Hopper%2C_USN_%28covered%29.jpg "img2")


To learn more about her, read this: http://www.biography.com/people/grace-hopper-21406809

## Compiler
Google what a compiler is and write two or three sentences on why that was so important for the advancement of computing.



## Ask Forgiveness
Have you ever heard the quote, “It's easier to ask forgiveness than it is to get permission.”? That was her.

![alt text](https://i2.wp.com/hopperboulder.com/wp-content/uploads/2019/03/Grace1-2.jpg?w=704&ssl=1 "img1")

This quote comes from an interview in the July 1986 CHIP’s Ahoy Magazine, the Department of the Navy’s Information Technology Magazine. She was at the cutting edge then and it is a testament to her vision how well this interview stands up to the test of time. Her passion for knowledge and innovation is the most important thing you can carry with you.

Read this: [http://www.doncio.navy.mil/chips/ArticleDtails.aspx?id=3563](http://www.doncio.navy.mil/chips/ArticleDtails.aspx?id=3563)

Write two or three sentences on how she viewed the impact of computers on the world.

## ROP
While there was a chance you knew what Hopper's meant, it is very unlikely that you have had any idea what Roppers meant, mostly because it is a word we made up to define a group of people who ROP. And if you have never heard of ROP, or Return Oriented Programming before, and.... that is not just okay, that is expected, because why on earth would you have known about an obscure programming topic before this exact moment in time.

To quote Wikipedia, "Return-oriented programming (ROP) is a computer security exploit technique that allows an attacker to execute code in the presence of security defenses such as non-executable memory and code signing by chaining together carefully chosen machine instruction sequences to get control of the stack..."

Don't worry; none of that should have meant anything to you. That would have made zero sense to me when I was sitting where you are sitting. 2 years into my journey, I would have understood about half of it. Now I can explain it and write basic ROP exploits, but that doesn't mean I can do it without a pile of references and examples.

While many other sites that attempt to teach this material assume you already know a great deal of knowledge, we take a different approach to make this challenging subject as approachable as possible. For all of the great resources out there, and all of the incredible pieces of training, nothing walks a complete beginner all the way through the process of developing a strong foundation in the fundamentals. Everyone wants to learn how to do stuff, but very quickly they realize that there is no way for them to learn everything. They’re not wrong, the vast and constantly expanding body of knowledge about this field makes it impossible for anyone to keep up. But what is most important for the beginner to realize is that with the proper knowledge of the fundamentals and a firm grasp on the hacker mentality, that irrepressible drive to learn and to do, nothing is too complex for them to learn if they put the time in.

By managing new your high expectations of yourself, providing constant feedback on your progress, and bringing you into the community, this is designed to minimize dropout rate while providing the best first thousand hours of a cyber security education possible.

## Core Tenets
This site is designed around a series of ideas that we think will make your experience as a learner as good as possible.

1. No initial expectation of knowledge
2. Everyone moves at their own pace
3. Understanding foundational theory comes before building technical skills
4. Developing fundamental technical skills lays the groundwork for success in any topic
5. Knowledge must be actionable
6. The measure of a community is how they treat those who are trying to gain entry
7. There is no such thing as being done learning

Anytime something on this site doesn't seem to be matching up with our core tenets, let us know so we can fix it. We will make as many possible mechanisms for you to help us improve our approach, the content, and the community of this site as possible. This site is a living entity and will change on a regular basis so that we can improve your experience.

# So What is ROP?
All you need to know right now is that ROP is an advanced exploitation technique which beats advanced defenses by chaining together code which was already in a program in order to perform unexpected behavior which gives an attacker control. That definition is good enough for now, but if you stick around with us, soon enough you will know what it means and eventually you will be writing exploits of your own. The critical bit for you to understand right now is that you take snippets of existing code, chain it back together in a new order, and then use those to jump to where you need to go next. As you go through this course you will do the same thing, reusing already learned information and arranging it to jump to new locations.

## Content

![alt text](https://news.yale.edu/sites/default/files/styles/horizontal_image/public/d6_files/YaleNews_hopper-grace.UNIVAC.102635875-CC_0.jpg?itok=4HL3ETlO "img3")

This curriculum was created based on inputs from members of the great Naval Academy classes of '15, '16, '17, and '18. I put this curriculum together by aggregating all of the guides on how to become successful in information security, took what I thought was important and added things of my own, mostly commentary that may or may not add value. To say that this is built on the backs of a hundred other guides would be an understatement, and I am forever grateful that I am part of an infosec community which has so many online resources. I specifically want to give a shoutout to the professors teaching Plebe Cyber at the Naval Academy, their SY201 course is the single best academic introduction to security in existence and I appreciate all of their guidance during my time with them. All attempts to cite source material have been made. This is the first iteration of the curriculum online and it should change drastically as I see what does and doesn't work, and the only way I will know is feedback from students like you.

## Feedback

After every section, we are going to ask for feedback. What did you like, not like, want changed, any thoughts. Just stream of consciousness it, the more information we get the better.

We can only get better if you tell us what you want changed, and you won't hurt our feelings. You can provide feedback over instant message on Slack, email to d.m.devey@gmail.com, or just to people in person. We just want you to learn and then give us feedback so we can learn.


## Support
Our site provides real time support through instant messaging, or you can hit us in Slack or on the forums. Whatever works, we are here for you.
