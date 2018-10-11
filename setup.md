---
layout: page
title: Setup
root: .
---

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
pwd
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
cp /workspace/hradxj/intro-linux.zip .
```
{: .language-bash}

Don't forget the dot at the end!

Now, type the following into the CLI and and press `ENTER`.

```
unzip intro-linux.zip
```
{: .language-bash}

This command will `unzip` the file `intro-linux.zip`. You will see that the `unzip` program creates some new subdirectories, and inflates a lot of files within those subdirectories. These are the files you'll be working with this morning.

Now, let's change directories, into the new directory that was created during the unzipping process. Type the following into the CLI and and press `ENTER`.

```
cd intro-linux
```
{: .language-bash}

Now, let's check that we are in the correct directory. Type the following into the CLI and and press `ENTER`.

```
pwd
```
{: .language-bash}
I would see the following:
```
/home/hradxj/intro-linux
```
{: .output}

In your case, it will be the same, except with your username.

Now, we are ready.

> #### Reference
> * [Using a Unix/Linux emulator (Cygwin) or Secure Shell (SSH) client (Putty)](http://faculty.smu.edu/reynolds/unixtut/windows.html)
{: .callout}
