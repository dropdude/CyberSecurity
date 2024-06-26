[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/c8uge2Vf)
# CECS 478 Lab: Buffer Overflow

## Assignment Description

This assignment focuses on buffer overflow attacks and how they can be carried out on poorly-programmed system programs. You may not be able to complete this assignment on a modern operating system, as modern compilers build canaries into code in order to prevent such a thing from occurring. I would recommend using an older Linux distribution in a virtual machine for this assignment (something prior to Linux kernel version 2.4), but you are welcome to attempt this on a modern OS and see if you can get it to work. Review the article [Smashing the Stack for Fun and Profit](http://phrack.org/issues/49/14.html) for a very good, detailed introduction on how to perform a stack smashing attack.

## Assignment

Given the following C code file, perform a stack smash on the [vuln.c](vuln.c) code file using a C program that you create named `exploit.c`. Your program should attempt to open up a reverse shell on the attacked program as root by exploiting the buffer (you can verify this by typing the command `whoami` on the resulting terminal). The [vuln.c](vuln.c) code must be compiled in its own, separate program and must not be altered from its original state.

Note: when running many versions of Linux, you may need to [disable some address randomization](http://gcc.gnu.org/wiki/Randomization).

## Deliverables

Submit your `exploit.c` to your git repository along with:

* A writeup (written in Markdown) of how you attempted the stack smashing attack.
* At least one screenshot of the output or result of a successful attack.
        * If you are not able to succeed with the attack due to OS constraints, detail that in your writeup and explain how you would go about performing such an attack on this system (along with your C code).

### Please note:

* Your writeup *must* be done in [Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) format and must be included in the repository as a separate file. View the file [`README.md`](README.md?plain=1) for an example of Markdown.
* Screenshots should be done in `*.jpg`, `*.png`, or `*.gif` formats, and be included individually as files in your repository (i.e. no binary ‘document’ with the images pasted inside). Screenshots which are too zoomed-in, which do not show your desktop, or are otherwise unidentifiable as belonging to you will not be counted.
* Screenshots *may* be linked in your Markdown file writeup if you wish to do so.

Your submission must follow the following rules, else *I will not grade it and you will receive a zero for the submission*:

* Do not use compression on your files.
* Make sure that all significant code is *commented* with your own explanations.
