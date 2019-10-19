Networking is the darkest art... and you may become an expert. Eventually. But all things considered, you will not be, and do not need to be an expert all the time. You become an expert on things when you need to be, when you have a challenge or a job or for whatever reason you need to become one of the world's leading experts in some bit of minutiae. There are people out there who are network wizards who do it for a living. Then there is everybody else who has to relearn everything every time they go in depth. What we will teach you here is scraping the minimum knowledge required to not need to Google everything. You will still Google everything, but this lets you get into the mix faster and will let you bullshit your way through most things. At the end of the day, you will never not need reference material and guides to work with networks.


* Read this whole thing. <https://www.digitalocean.com/community/tutorials/an-introduction-to-networking-terminology-interfaces-and-protocols>
* Read this whole thing. <https://commotionwireless.net/docs/cck/networking/learn-networking-basics/>
* Watch this: <https://www.youtube.com/watch?v=3QhU9jd03a0&list=PL8dPuuaLjXtNlUrzyH5r6jN9ulIgZBpdo&index=29> I really like this series. It's all pretty good.

1. What is a packet? What is encapsulation and how does it work?
2. What is a protocol? What are examples of protocols?
3. What is the OSI model? What is the TCP/IP model? Why are they different?
4. What is a MAC address? What is an IP address? What is the difference?
5. Describe the client-server relationship.
6. What are ports for? How are ports assigned?

* Read this: Specifically, 1.1-1.4, 1.9, <https://intronetworks.cs.luc.edu/current/html/intro.html>
1. What is datagram forwarding? How do forwarding tables work?
2. In MAC addresses, how can you tell who the manufacturer of the device is?
3. What are multicast and unicast and what are the differences?
4. What is a switch?
5. Who assigns IP addresses?
6. What is a LAN? How do IPs on a LAN communicate? How do IPs not on the same LAN communicate?
7. What is packet fragmentation?
8. What is the difference between IP forwarding and datagram forwarding?
9. How does the internet backbone work? Use the word BGP in your answer.
10. What is TCP and UDP, and what are the differences?

* DNS is hard, read this: <https://code.tutsplus.com/tutorials/an-introduction-to-learning-and-using-dns-records--cms-24704>
1. What is DNS?
2. Why does it exist?
3. How does it work?

### Wireshark:
 * Work through the NewBoston Wireshark tutorial. No need to watch all of it, or at regular speed. Try 1.5 speed (or 2x) and bounce around to learn as much as you can.
    * <https://www.youtube.com/watch?v=flDzURAm8wQ&list=PL6gx4Cwl9DGBI2ZFuyZOl5Q7sptR7PwYN>

 I'm sorry. This deserves its own thing but I haven't made it yet.

### Cyber Aces
When you finish a tutorial, screenshot it and submit.

1. Introduction and Layer 1  <https://tutorials.cyberaces.org/tutorials/view/2-1.html>
2. Layer 2 - Data Link <https://tutorials.cyberaces.org/tutorials/view/2-2.html>
3. Layer 3 - Network, Part 1: Addressing & Masking <https://tutorials.cyberaces.org/tutorials/view/2-3.html>
4. Layer 3 - Network, Part 2: Routing <https://tutorials.cyberaces.org/tutorials/view/2-4.html>
5. Layer 3 - Network, Part 3: Communication <https://tutorials.cyberaces.org/tutorials/view/2-5.html>
6. Layer 4 - Transport <https://tutorials.cyberaces.org/tutorials/view/2-6.html>
7. Layers 5 & 6 - Session and Presentation <https://tutorials.cyberaces.org/tutorials/view/2-7.html>
8. Layer 7 - Application <https://tutorials.cyberaces.org/tutorials/view/2-8.html>
9. Inter-Layer Communication & Conclusions <https://tutorials.cyberaces.org/tutorials/view/2-9.html>

## RFCs
RFCs or Request for Comments, is the way that the internet develops standards. Read this to learn more: <https://www.lifewire.com/what-is-internet-request-for-comments-rfc-4092366>

Now the important thing is how to read an RFC.

* From the organization that approves RFCs. <https://www.ietf.org/blog/how-read-rfc/>
* This is short and sweet but applies to just about any technical document: <https://softwareengineering.stackexchange.com/questions/179022/how-does-one-read-rfcs-and-similar-documents>
* Skim the HTTP RFC to answer a few questions: <https://www.rfc-editor.org/rfc/rfc7231.txt>

1. Is this an official RFC? What RFC did it update?
2. What does this RFC give guidance on how to do?
3. What are the 5 families of response status codes?  
4. What is a GET request and what does it look like?
5. What is a User-Agent?
6. What RFC guides "cache-control" in a header?

* Skim the DNS RFC to answer questions. I won't give you the RFC for this, go find it.

1. What is the format of a DNS Resource Request (RR) datagram?
2. What does RDATA do?
3. How many bytes (not octets) can be placed in an experimental NULL RDATA format?
4. How many bytes are messages carried by UDP restricted to?
5. What is the TC bit?
6. Would you describe the TC bit as... boolean? What is a bool?
7. In the header of a message, how many bits from the ID field is the TC bit?

Congratulations, you are, at this exact moment in time, the world's 2nd most knowledgeable person about TC bits. Alright, now time to forget that and move on to learning more important things, like reading the "Standard for the Transmission of IP Datagrams on Avian Carriers" for fun. I promise this one is shorter. <https://www.rfc-editor.org/rfc/rfc1149.txt>

## TCP-IP Book

The book TCP-IP Illustrated is the bible. You should buy it at some point. For now, just use this copy. <http://www.r-5.org/files/books/computers/internals/net/Richard_Stevens-TCP-IP_Illustrated-EN.pdf>. I had a hard copy for a while, but I left it behind with my security team when I graduated. I hope it's getting good use now. Anyway, any time you have a question about a protocol, find it here, and do some Google. Together, you are unstoppable. There are two other books in the series, but this is the book that you will use the most.

## Conclusion

Networking is really hard, but hopefully this exposure gave you enough. The biggest takeaway you can have is using Google and RFCs effectively to solve your problems. The good news is that when it comes to network problems, someone has already seen it before and asked the question. And, as the joke goes, it is always a DNS problem.
