* Intro to Linux
       * https://linuxjourney.com
       * Story of Linux (Cathedral and the Bazaar)
       * Varieties of Linux
       * Getting Started
       * Command Line
           * Code Academy Command Line
       * Undertstand the Unix filesystem
* Ubuntu Intro
      * https://www.cybrary.it/course/comptia-linux-plus
      "Unix will give you enough rope to shoot yourself in the foot. If you didn't think rope would do that, you should have read the man page."
       * Know the locations and purposes of important configuration files
         * What are dotfiles
 * Know the function of all of the commands listed in the intro section, and use them
         * Know the syntax and semantics (including some important switches) to all commands marked with an asterisk in the intro section by memory
	 * Know how to read and use a manpage, and explain the various parts that make up a manpage

       * User Management
       * Permissions
       * Packages
       * Init/SystemD
* Command Line Basics
* Know exactly what the command line is. *What is really is*
* http://linuxcommand.org/tlcl.php (pg 26-30)
* Understand the filesystem of the Unix system.
* http://linuxcommand.org/tlcl.php (pg 31-36)
* Big emphasis on the important commands in Unix. Contains the bulk of command explanation in this section of qualification.
* pwd,ls,cd,cat,man,apt-get/aptitude,chgrp/chown/chmod,cp,cut,diff,dmesg,echo,export,file,find,grep,gzip/bzip2/unzip/tar,head,ifconfig,jobs,kill,less,ln,mkdir,mkfifo,mount/umount,mv,netstat,nslookup,open/gnome-open,passwd,ping,rm,scp,sort,ssh,sudo,su,tail,touch,top,traceroute,vi,whoami,xargs,alias
* http://ss64.com/bash/
* http://linuxconfig.org/linux-commands 
* http://linuxcommand.org/tlcl.php (pg 37 - 76)
* Basic System Administration
* Accounts, groups and permissions in Unix.
* http://linuxcommand.org/tlcl.php (pg 112 - 131)
* Important directories and configuration files.
* http://www.tecmint.com/linux-directory-structure-and-important-files-paths-explained/
* http://www.dba-oracle.com/linux/important_files_directories.htm. 
* Using a package manager.
* http://linuxcommand.org/tlcl.php (pg 190 - 199)
* System Boot and the startup services
* http://www.linux.com/learn/tutorials/404619-manage-system-startup-and-boot-processes-on-linux-with-upstart 
* Man Pages
* Explain what manpages are and why they are important.
* https://en.wikipedia.org/wiki/Man_page 
* Explain the different manpages sections.
* https://www.kernel.org/doc/man-pages/ 
* How to use man pages
* http://linuxcommand.org/reading_man_pages.php
* http://linuxcommand.org/tlcl.php (pg 69-71)
* Challenge: Explain the sections of manpages and the type of information in man pages.
* Pipelines and Redirects
* Explain what pipelines are and what they are used for.
* http://linuxcommand.org/tlcl.php (pg 83-89)
* Three channels (stdin, stdout, stderr).
* http://linuxcommand.org/tlcl.php (pg 77)
* https://en.wikipedia.org/wiki/Standard_streams 
* Explain what redirects are and what they are used for.
* http://linuxcommand.org/tlcl.php (pg 77-81)
* Magical redirects.
* http://tldp.org/HOWTO/Bash-Prog-Intro-HOWTO-3.html 
* Demonstrate the power of the two commands being used together.
* http://ryanstutorials.net/linuxtutorial/piping.php 
* Explain the alternative tee command.
* http://linuxcommand.org/tlcl.php (pg 88-89)
* http://linux.101hacks.com/unix/tee-command-examples/ 
* Challenge: Cyberstakes Redirect problem
* Challenge: The Great Command Line Challenge
* https://opensource.com/life/15/7/pipe-dreams 
* FIFO and NC listener
* The many wonders of Netcat. Netcat fundamentals, file transfer, flags and backdoor shells.
* https://www.sans.org/security-resources/sec560/netcat_cheat_sheet_v1.pdf
* http://www.tutorialspoint.com/unix_commands/nc.htm 
* http://www.binarytides.com/netcat-tutorial-for-beginners/ 
* Introduction to named pipes and their uses
* http://linuxcommand.org/tlcl.php (pg 522-523)
* http://www.tldp.org/LDP/lpg/node15.html
* http://www.linuxjournal.com/article/2156
* Examples of how to use FIFO and how to make tasks easier.
* Challenge: Demonstrate a file transfer using NC
* Challenge: Demonstrate a backdoor and reverse backdoor shell
* Cron Jobs
* Understand that cron is a daemon used to run scripts at a specified time.
* http://www.unixgeeks.org/security/newbie/unix/cron-1.html 
* Using the crontab command
* http://kvz.io/blog/2007/07/29/schedule-tasks-on-linux-using-crontab/ 
* Creating scripts to be run by cron.
* Challenge: Create a cronjob running every 5 minutes to detect if a file has been changed.
* Defense
* PS command
* Understand basic idea of a process.
* http://linuxcommand.org/tlcl.php (pg 132-145)
* Difference between foreground and background process.
* http://linuxcommand.org/tlcl.php (pg 132-145)
* http://www.tutorialspoint.com/unix/unix-processes.htm
* Listing process and understanding details from the output.
* http://linuxcommand.org/tlcl.php (pg 132-145)
* Using the ps, kill, and top commands
* http://linuxcommand.org/tlcl.php (pg 132-145)
* http://www.tutorialspoint.com/unix/unix-processes.htm 
* Understand parent and child processes.
* http://www.tutorialspoint.com/unix/unix-processes.htm  
* Understand zombie and orphan processes.
* http://www.tutorialspoint.com/unix/unix-processes.htm 
* Difference between Job ID and Process ID.
* http://www.tutorialspoint.com/unix/unix-processes.htm 
* Challenge: Pull up current processes on your machine and explain the output
* netstat
* Understand that the command netstat is a tool for checking network configuration and activity.
* http://linuxcommand.org/tlcl.php (pg 222-223)
* Understand the common configurations encountered from netstat output and what is malicious or not.
* http://www.binarytides.com/linux-netstat-command-examples/ 
* Bash Scripting (In automation as well)
* Understand when to use BASH scripting.
* Understand structure of script, special characters and variables.
* Understand internal variables, manipulating strings, parameter/command substitution, loops, and arithmetic expansion.
* More stuff depending on how indepth we want to go.
* http://www.tldp.org/LDP/abs/html/ (all you really need)
* http://linuxcommand.org/tlcl.php (pg 377-384) (*this as well)
* Challenge: Write a shell script that, given a file name as the argument will write the even numbered line to a file with name evenfile and odd numbered lines in a text file called oddfile.
* Environment
* Understand what the environment consists of.
* http://linuxcommand.org/tlcl.php (pg 148-159)
* http://www.tutorialspoint.com/unix/unix-environment.htm 
* Explain various environment variables.
* http://linuxcommand.org/tlcl.php (pg 148-159)
* http://www.tutorialspoint.com/unix/unix-environment.htm 
* Understanding alias and configuration files in environment (.bashrc).
* http://linuxcommand.org/tlcl.php (pg 148-159)
* http://www.tutorialspoint.com/unix/unix-environment.htm 
* Board Question
* Importance of LD_PRELOAD and PATH.
* http://stackoverflow.com/questions/426230/what-is-the-ld-preload-trick (simple explanation of goal)
* https://cbednarski.com/articles/understanding-environment-variables-and-the-unix-path/ 
* Board Question
* Grand Challenge: Complete OverTheWire Bandit Set

* Ubuntu key bindings
* basic latex
	 	* Basically tutorials point will teach you anything, this time, latex (pronounced latech)
		* nerds lose their minds over this stuff
		   * https://www.latex-tutorial.com/tutorials/
		* https://www.sharelatex.com/
		* Whats the hacker ethic???? 
		    * Install latex font in word 
		        * https://tex.stackexchange.com/questions/8308/make-ms-word-document-look-like-it-has-been-typeset-in-latex
		    
                
                 
	 * Text Fu
	        * Dont use mice!!!
		* For anything, but especially not text
		* Learn one text editor
		* Learn one IDE
		* Also, learn how to customize editors
       		* Linux
		   * https://www.xkcd.com/378/
		   * http://www.explainxkcd.com/wiki/index.php/378
		   * nano
		      * https://www.howtogeek.com/howto/42980/the-beginners-guide-to-nano-the-linux-command-line-text-editor
		   * emacs
		      * http://www.jesshamrick.com/2012/09/10/absolute-beginners-guide-to-emacs/
		      * This is the best one
		   * vim
		      * https://www.linux.com/learn/vim-101-beginners-guide-vim
		      * Or this one.
		      * https://vim-adventures.com/
		      * make a vmrc dotfile!
                     * Dotfiles
	   * https://en.wikipedia.org/wiki/Hidden_file_and_hidden_directory
	   * how do they work? 
	   * why is this there
	   * technical debt
	      * https://en.wikipedia.org/wiki/Technical_debt
	   * what do they do
	      * https://medium.com/@webprolific/getting-started-with-dotfiles-43c3602fd789
	   * bashrc
	   * vimrc
	   * tmuxrc
	   * git
		   * cat
		      * https://www.linux.com/blog/using-cat-text-editor
		      * There is more than one way to skin a cat
		   * Good IDE
		   * either way, choose vim or emacs and use it for everything. Ever.
               
               
* S&A 
       * one liner
       * linux scripting
          * bash script vs shell script
             * https://askubuntu.com/questions/172481/is-bash-scripting-the-same-as-shell-scripting
             * Why are things the way they are? Weird historical stuff. Get used to it.
       * Basic Regex
       * Sed, Awk, Grep
       * Netcat magic
       * Send an email from command line
