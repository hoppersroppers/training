What is an operating system? From your current understanding, you have a pretty good idea about how to use Windows and Linux. However, what we are about to go over is what is actually occurring under the hood. For the every day user of a computer, there is no need to know just about any of this, but without a strong base in the things that operating systems do for you and how they do them, you'll have a lot of misconceptions and blind spots that will limit your ability to grow. The technical word for this is "abstraction". Operating Systems abstract away the requirement for end users to be able to program or know how to set up a network connection. Everything is handled for the average user by the Operating System... but you are no longer the average user and you are going to need to get everything you can out of the system that you are using. And that is why you need to understand operating systems. At some point you will likely take a class specifically on this, but for now, this gives you enough to be dangerous. In this section we will go over the basics of operating systems as well as work towards becoming a Windows and Linux power user.

## Operating Systems
* Work through this entire guide and answer questions as you go.  <https://www.tutorialspoint.com/operating_system/index.htm>. You will also need to use other resources, I recommend wikipedia, but there are plenty of other amazing resources out there on this topic. During this section, I highly recommend you chat up teachers in order to ask questions and get clarification.

1. Describe what an operating system (OS) is responsible for. This is a trick question, it's everything.
2. What are the different types of OS? Which one is most common?
3. What is a kernel? What does "abstraction" mean?
4. What is the difference between user level and kernel level?   
5. What does an OS do with memory?
6. What is process address space?
7. What is "swapping"?
8. What is fragmentation?
9. What does de-fragmentation do? (Fun fact, modern operating systems will do this for you... just another thing abstracted away)
10. What is multi-programming in regard to CPU execution?
11. What is the difference between a program and a process?
12. What is processor management?
13. How does process scheduling work?
14. What is a driver?
15. What is device management?
16. What is file management?
17. What is an I/O operation? (Hint I/O stands for input/output)
18. What is an interrupt?


* Read this <https://www.usna.edu/Users/cs/wcbrown/courses/si110AY13S/lec/l04/lec.html>
* Do the homework and submit screenshots. <https://www.usna.edu/Users/cs/wcbrown/courses/si110AY13S/lec/l04/hw/hw.pdf>

* Read this <https://www.usna.edu/Users/cs/wcbrown/courses/si110AY13S/lec/l05/lec.html>


* Read the wiki <https://en.wikipedia.org/wiki/File_system> down to the end of 'Aspects of File Systems'
1. What is a file system?
2. What is an API? Why are they useful?
3. What is a directory?
4. What is metadata? Why is it important to have metadata?
5. What is disc partitioning?

## The Operating Systems

Alright, that wasn't enough for most of it to make sense, but it's over now. Sorry to bore you with the rough stuff. Now we are on to the stuff that you will be able to immediately put into use, becoming a power user. The more you know about the operating system you work off of, the more efficient you will be, which lets you learn more and do more which makes you better, which makes you more efficient....

What I am trying to say is get really good at Windows and Linux and your life becomes better.

Here is an obligatory comic strip about "The Holy Wars", Windows, vs Linux. <https://dilbert.com/strip/1995-06-24>. You'll be starting with Windows. You've used it for the last decade or two of your life, but you ain't seen nothing yet.

### Windows
* History of Windows (and Microsoft)
   * I actually love these videos. <https://www.youtube.com/watch?v=JmtPWvT1vp8>
   * Part Two: <https://www.youtube.com/watch?v=XDE7QPMBQAU>

For all tutorials, complete the tutorial section and screenshot something showing your completion and submit.

* Command Line Basics
   * <https://tutorials.cyberaces.org/tutorials/view/1-2-3.html>
   * Windows Linux Command Line
      * <https://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/>
   * Powershell
      * <https://tutorials.cyberaces.org/tutorials/view/3-3-1.html>
   * .bat Script
      * <https://www.howtogeek.com/263177/how-to-write-a-batch-script-on-windows/>
* File System   
         * <https://tutorials.cyberaces.org/tutorials/view/1-2-4.html>
         * <https://www.2brightsparks.com/resources/articles/understanding-file-attributes.html>
         * <https://www.wideanglesoftware.com/blog/windows/8-tips-free-up-space-on-computer.php>
         * <https://resources.infosecinstitute.com/category/computerforensics/introduction/areas-of-study/digital-forensics/media-file-system-forensics/>
* Users and Groups
   * <https://tutorials.cyberaces.org/tutorials/view/1-2-5.html>
   * Create a guest user for your Windows machine and submit a screenshot
* Policies and Credential Storage
   * <https://tutorials.cyberaces.org/tutorials/view/1-2-6.html>
* Registry
   * <https://tutorials.cyberaces.org/tutorials/view/1-2-7.html>
* Networking and Sharing
   * <https://tutorials.cyberaces.org/tutorials/view/1-2-8.html>
* Services and Processes
   * <https://tutorials.cyberaces.org/tutorials/view/1-2-9.html>
   * <https://www.online-tech-tips.com/windows-10/windows-10-task-manager-overview-part-i/>
   * Virtual Memory
    * On Windows, check to see how much RAM you are using with your virtual machine. Google how to do this.
    * Check to see how much RAM is being used by your VM and what the CPU utilization looks like. Google again.
    * Increase RAM allocated to Virtual Machine.... Yep.
    * Check back on your VM to see CPU utilization.
    * Decrease VM RAM to whatever is necessary. Now you can use this whenever you want to prioritize the speed of processing in your VM. Just bump your VM RAM, run your process, then reallocate back to Windows once it is complete. Boom, you are basically an operating system now.
* Boot Process
    * <https://social.technet.microsoft.com/wiki/contents/articles/11341.windows-7-the-boot-process-explained.aspx>
    * What the F is a UEFI? <https://www.howtogeek.com/56958/htg-explains-how-uefi-will-replace-the-bios/>
* Windows
    * <https://www.howtogeek.com/123646/htg-explains-what-the-windows-event-viewer-is-and-how-you-can-use-it/>
    * Turn on Sysmon
          * <https://docs.microsoft.com/en-us/sysinternals/downloads/sysmon>
          * Install Tay's Sysmon config <https://github.com/SwiftOnSecurity/sysmon-config>
          * <https://resources.infosecinstitute.com/category/computerforensics/introduction/areas-of-study/digital-forensics/operating-system-forensics/>
          * We are not going to go over forensics, but read over this poster and look at all the artifacts that are created by Windows. <https://www.sans.org/security-resources/posters/windows-forensic-analysis/170/download>


### Linux
* History
   * Read this: <https://dwheeler.com/secure-programs/Secure-Programs-HOWTO/history.html>
   1. What is the difference between Unix and Linux?

   For all tutorials, complete the tutorial section and screenshot something showing your completion and submit.

* Command Line
   * <https://tutorials.cyberaces.org/tutorials/view/1-1-3.html>
   * <https://tutorials.cyberaces.org/tutorials/view/3-2-1.html>
* Users and Groups
   * <https://tutorials.cyberaces.org/tutorials/view/1-1-4.html>
   * Create a guest user for your Linux VM. You'll have to Google this.
* Applications and Services
   * <https://tutorials.cyberaces.org/tutorials/view/1-1-5.html>
   * <https://www.howtogeek.com/107217/how-to-manage-processes-from-the-linux-terminal-10-commands-you-need-to-know/>
* Files and Permissions
   * <https://tutorials.cyberaces.org/tutorials/view/1-1-6.html>
   * <https://www.makeuseof.com/tag/manage-ubuntu-hdd-disk-utility/>
* Boot Process
     * <https://www.crybit.com/linux-boot-process/>
* Logs
     * <https://www.linux.com/learn/sysadmin/viewing-linux-logs-command-line>
     * <https://www.sandflysecurity.com/wp-content/uploads/2018/11/Linux.Compromise.Detection.Command.Cheatsheet.pdf>
