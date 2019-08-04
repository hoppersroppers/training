* History of Computers
   * Read this: http://www.explainthatstuff.com/historyofcomputers.html
    
## Storage Density
   * https://www.dataversity.net/brief-history-data-storage/
   * All that is good information, but the critical thing is that it's all just been progressively smaller ways to store data
   * Nowadays, we use electricity to store 1s and zeros. 
   * It is always useful to know more about electricity https://learn.sparkfun.com/tutorials/what-is-electricity
   
   1. Write a brief bit about the importance of storage density. 
    
## Telecommunication Basics
   * Read all of this. 
   * https://en.wikipedia.org/wiki/Telecommunication
         * https://en.wikipedia.org/wiki/Naval_flag_signalling
         * https://en.wikipedia.org/wiki/Flag_semaphore
         * https://en.wikipedia.org/wiki/Morse_code
         * https://en.wikipedia.org/wiki/ARPANET
             * https://en.wikipedia.org/wiki/Packet_switching
   * If you haven't noticed yet, the military cares a lot about sending information. 
   
   * So what did we learn there? 
   1. Write a brief bit about the importance of bits per second.
   2. Write a couple sentences about what ARPANET was.
   
   * How do these ones and zeros work https://learn.sparkfun.com/tutorials/binary
   * What can you represent with all those 1s and 0s. 
   * Do this https://code.tutsplus.com/articles/number-systems-an-introduction-to-binary-hexadecimal-and-more--active-10848
   * Also, hey, what is ascii? This is ascii. https://en.wikipedia.org/wiki/ASCII
   * Also hey, what is hex? https://en.wikipedia.org/wiki/Hexadecimal
    
   0. How many bits are used for each character in ASCII?
   1. "01101000 01100101 01101100 01101100 01101111 00100001" is in binary. Conver it back to ASCII. Do it by hand using the chart.
   2. Alright. Now. Convert 17 in Ascii to Binary and Hex. Do it by hand.
   3. Convert "Go Navy" to Octal, Hex, and Binary. Yes. By hand.
   4. What is does "c2l4dHlmb3Vy" translate to from Base64?
  
* Read this https://www.usna.edu/Users/cs/wcbrown/courses/si110AY13S/lec/l01/lec.html
* Do the HW https://www.usna.edu/Users/cs/wcbrown/courses/si110AY13S/lec/l01/hw/hw.pdf

* Read this https://www.usna.edu/Users/cs/wcbrown/courses/si110AY13S/lec/l02/lec.html
* Do the HW https://www.usna.edu/Users/cs/wcbrown/courses/si110AY13S/lec/l02/hw/hw.pdf

* It is annoying to do that by hand, but it does help. Here is a tool so that you never have to do that again. https://gchq.github.io/CyberChef/. Fun fact, it is released by GCHQ, Britain's version of the NSA. Great tool and very very useful. There are about a thousand uses for this thing, you can find a bunch on GitHub.

   
## Digital Logic Basics
   * Digital logic: https://learn.sparkfun.com/tutorials/digital-logic
   * Read this one too:  https://web.archive.org/web/20061008134026/http://www.facstaff.bucknell.edu:80/mastascu/eLessonsHTML/Logic/Logic1.html
    
    
    1. Explain how digital logic is an essential part of computing. 

# Hardware Basics

* Using Google, explain all these things. Put it in a text file.

1. Explain what a motherboard is
2. PCI Slot
3. CPU 
4. Why is a fan needed?
5. RAM
6. Hard Drive
7. Optical Hard Drive
8. Solid State Hard Drive     
9. Graphics Card


# Levels of Code
## Machine Code and Assembly Code

In order to be executed on a CPU, code must be written in a way that is understood by the CPU. This is called 'Machine Code' and consists of 1s and 0s. As a note, there are various families of CPU architectures which require different machine codes to operate properly. Humans don't like 1s and 0s as much as computers so we prefer to abstract ourselves away from the bits as far as possible. The first step of this is something called an "Assembler". You can generally think of an assembler as a piece of code written for a specific type of CPU that does a 1 for 1 exact translation of code into binary that can be executed. 

I like this video: https://www.youtube.com/watch?v=wA2oMRmbrfo

Assemblers do a 1 for 1 translation, but what if we are looking for something that can optimize or simplify the work needed to be done by the programmer? In that case we would need something called a compiler. A compiler is a computer program that translates computer code written in one programming language (the source language) into another programming language (the target language). This allows the programmer to save huge amounts of time and spend more time doing and less time working. 

Hey, read this about our namesake Grace Hopper and the first compiler: https://history-computer.com/ModernComputer/Software/FirstCompiler.html

Watch this: https://www.youtube.com/watch?v=IhC7sdYe-Jg

Some day, you will probably write a compiler so all of the things you just learned about makes more sense to you. Or you can not. I did it once. Didn't get as much out of it as people told me I would. 

______________

http://nongnu.askapache.com/pgubook/ProgrammingGroundUp-1-0-booksize.pdf
