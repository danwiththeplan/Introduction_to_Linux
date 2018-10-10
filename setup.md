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

Firstly, check that you really are in your personal home directory. Type the following into the CLI and press `ENTER`.

```
pwd
```
This is a Linux command that asks "what directory am I currently in" (or "**p**resent **w**orking **d**irectory" for short).
Everyone will see a different output, because the personal home directory is named after your username, and everyone has a 
different username. For me, the command would output the following:

```
/home/hradxj
```
..because my PFR username is `hradxj`.

Now we need to create a new subdirectory, to put some test data into. Type the following into the CLI and press `ENTER`.

```
mkdir intro-linux
```
Now let's move into that directory.  Type the following into the CLI and press `ENTER`.

```
cd intro-linux
```
Check that you really are in the correct directory. Type the following into the CLI and press `ENTER`.

```
pwd
```

You should see the following:
```
/home/your_PFR_username/intro-linux
```

Now let's copy the test data.. which is sitting in Dan's personal workspace.. into the `intro-linux` directory.
Type the following into the CLI and press `ENTER`.

```
cp /workspace/hradxj/data-shell.zip .
```
Don't forget the dot at the end! 
Now, check that you do have a file called `data-shell.zip` in your current directory.
Type the following into the CLI and press `ENTER`.
```
ls
```
You should see the following:
```
data-shell.zip
```

Now, we are ready.

> #### Reference
> * [Using a Unix/Linux emulator (Cygwin) or Secure Shell (SSH) client (Putty)](http://faculty.smu.edu/reynolds/unixtut/windows.html)
{: .callout}
