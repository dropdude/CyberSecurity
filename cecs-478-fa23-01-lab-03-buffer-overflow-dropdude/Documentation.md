# CECS 478 Lab: Buffer Overflow

## Assignment Documentation

Steps taken to finish assignment

## Setting up VM

Decided to go with Kali Linux and got a VM off the kali website.

## Remove safety feature

Watched a youtube video on how to remove the safty ffeatures to perform a smash the stack attack.

Disabled ASLR by using the command in http://gcc.gnu.org/wiki/Randomization

## Performing the smash the stack

Following the instructionss for smashing the stack. I started with the exploit1 to see if it works with vuln.c file.

First running vuln.c it asked for badfile

After trying to compile it with exploit it gave error of strlen is unknown. Downloading string.h library to kali.

Unsure if the Aslr might be the issue or another issue is making it difficult to compile.
## What I would do if I could get it to work

A issue i found that could lead to problems is that some even performed correctly. The still wont get root access.

This is because to have to setuid to 0

I would have to see how the program responds and if I still didnt have root access I would implement this fix.

