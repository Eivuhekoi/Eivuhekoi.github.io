---
layout: default
---

# Command line course

The command line course is an eight week long university course attendable at Helsinki University. It teaches attendants about the usefull features of the command line interface, primerily on Unix machines and for linguistic applications.  

## Brief synopsis of the areas covered each week.

### Week 1

General introductions to the Unix command line environment, as well as setting it up on non Unix operating systems. In addition it covers terminal based text-editors.

### Week 2

Introduction to the Unix filesystem, as well as teaching how to navigate it using the command line. In addition this week covers managing and viewing files on via the command line, as well as giving a brief introduction to the Secure Shell, or ssh, and a few commands using it.

### Week 3

Basics of corpus processing on the command line, as well as an introduction to different character encodings.

### Week 4

Expanding on the previous weeks themes of corpus processing on the command line by introducing more advanced commands such as `sed`

### Week 5

Introduction to writing shell-scripts, and how they can be used to automate many command line tasks. Particularly the previously taught ways of converting text files into frequency tables was useful in my opinion.  
In addition this week also covered *configuration* files via introductin the **.bashrc** file that gets read when an interractive instance of the Bourne Again Shell (Bash) is started.

### Week 6

Introduced installing software, and using makefiles. In my opinion the latter was more useful for me personally as I already knew about installing software, and the methods given didn't work that well due to my particular choice of Linux distribution. However, after this I have startead using makefiles for various purposes.  
An example of a makefile instruction would be:
```make
%.freq: %.no_md.txt
	bin/freqlist.sh $< $@
```
Which tells the Makefile to run the `bin/freqlist.sh` script-file if files ending with `.freq` for a given list in the targets of the make file are not found. In addition it marks that for this make-tast to be performed on a file, a `.no_md.txt` file of the same name should exist. If if does not, then the make-tast for it is run if provided in the Makefile.

### Week 7

Introduction to version control software via learning Git. Personally this was also among the most useful weeks of the course, as I wasn't familiar with how to properly utilize git despite using it for many of my projects.

### Week 8

The final project was an introduction to creating websites to be hosted on github.io. You are currently reading one.
