---
layout: page
title: Setup
root: .
---
## Welcome to the powerPlant summit Introduction to Linux session.

Let's start with some details on how to follow the lesson, how to ask for help, and some useful external resources.

>It's important to acknowledge that this lesson was adapted from the [Software Carpentry shell-novice](http://swcarpentry.github.io/shell-novice/) lesson and that many people have contributed to development of this lesson, most of whom have nothing to do with PFR. If you are interested, maintainers and contributors are listed in the [github repository](https://github.com/danwiththeplan/Introduction_to_Linux).

## How to follow the lesson

The lesson mostly involves entering specific commands into the **C**ommand **L**ine **I**nterface (referred to as the **CLI** from now on). For most people the CLI will be the program **Putty**. 

When you see a box with a purple band on the left, this is a *command* that you'll need to enter into the CLI. The *command* is the bit after the *prompt* (which in this case is a `$`). 
Here's an example (but don't enter this into the CLI right now):
~~~
$ somecommand
~~~
{: .language-bash}

There are a few ways you can enter the command.


**First, you can simply type the command.** It should be entered *exactly as written*, including dots and spaces. It's important to note at this point that *Linux is case-specific*... so entering a `lowercase` command in `UPPERCASE` won't work. You'll learn some quicker and more useful ways to type commands as the lesson progresses.


**Secondly, you can cut-and-paste the command.** This can be done in two ways:


1) Highlight the text you wish to cut and paste, press `CTRL-C`, select the Putty window, and Right-click on your mouse.


2) Highlight the text you wish to cut and paste, press `CTRL-C`, select the Putty window, and press `SHIFT-Insert`.


When you see a box with a black band on the left, this is an *output* that you should expect to see in the CLI, usually after entering a *command*. Here's an example:

~~~
some expected output
~~~
{: .output}

## How to ask for help

To begin the lesson, please follow these steps:

1. Obtain a Green and Pink sticker.
2. You should have already installed a command-line interface to powerplant (for most people, this is [Putty](https://powerplant.pfr.co.nz/guide/cli). If you have not, please put up a pink sticker and we will try to help.
3. Open a Putty terminal and log in to powerplant.
3. When you log in to powerplant, you automatically start in your personal home directory. We need to create a new 
subdirectory and copy some files into it. This involves some commands that we'll learn more about as the lesson progresses.
So, don't worry if you don't quite know what you're doing here.

**First, check that you really are in your personal home directory.**

Type the following into the CLI and press `ENTER`.

~~~
$ pwd
~~~
{: .language-bash}

This is a Linux command that asks "what directory am I currently in" (or "**p**rint **w**orking **d**irectory" for short).
Everyone will see a different output, because the personal home directory is named after your username, and everyone has a 
different username. For me, the command would output the following:

~~~
/home/hradxj
~~~
{: .output}

..because my PFR username is `hradxj`. 


**Now let's copy the test data.. which is sitting in Dan's personal workspace.. into your personal home directory.**

Type the following into the CLI and press `ENTER`.

```
$ cp /workspace/hradxj/intro-linux.zip .
```
{: .language-bash}

Don't forget the dot at the end!

Now, type the following into the CLI and and press `ENTER`.

```
$ unzip intro-linux.zip
```
{: .language-bash}

This command will `unzip` the file `intro-linux.zip`. You will see that the `unzip` program creates some new subdirectories, and inflates a lot of files within those subdirectories. These are the files you'll be working with this morning.

Now, let's change directories, into the new directory that was created during the unzipping process. Type the following into the CLI and and press `ENTER`.

```
$ cd intro-linux
```
{: .language-bash}

Now, let's check that we are in the correct directory. Type the following into the CLI and and press `ENTER`.

```
$ pwd
```
{: .language-bash}
I would see the following:
```
/home/hradxj/intro-linux
```
{: .output}

In your case, it will be the same, except with your username.

Now, we are ready. Please put up a green sticker if you've got to this point.

> #### Reference
> * [Using a Unix/Linux emulator (Cygwin) or Secure Shell (SSH) client (Putty)](http://faculty.smu.edu/reynolds/unixtut/windows.html)
{: .callout}
