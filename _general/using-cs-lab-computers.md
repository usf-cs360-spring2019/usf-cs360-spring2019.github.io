---
title: Using CS Lab Computers
navbar: Guides
layout: default
---

You must use your CS account and CS lab computers (remotely or locally) to verify homework and projects.

## Account Basics

Your CS account shares the same username as your myUSF account, but different passwords. You should use your CS account for the following purposes:

  - Logging into the computers in the CS classrooms (Harney 142 and LS G12).

  - Logging into the computers in the CS labs (Harney 413).

  - Logging into the lab computers remotely via SSH.

Alternatively, you use your myUSF username and password to login into myUSF, Canvas, access your `@dons.usfca.edu` email, and other university-wide resources.

## Username and Password

Your CS account username will always be the same as your myUSF username. You can determine your username by looking at the part before `@dons.usfca.edu` in your USF email address. For example, if my email address is `sjengle@dons.usfca.edu` then my username will be `sjengle`.

Your initial password will be the LAST six digits of your student ID. Since your student ID is 8 digits, remove the first two digits from your student ID (usually `20...`) and use the remaining digits as your password. For example, if your student ID is `20123456`, then your initial password will be `123456`.

You should [change your password](https://www.cs.usfca.edu/support.html#password) after logging in for the first time.

## Local Access

If you are physically in one of the CS Labs, you can log into one of the lab computers running Linux directly using your username and password.

## Remote Access

If you want to access one of the CS Lab computers remotely (for example, from home or off-campus), you must [login using SSH](http://www.cs.usfca.edu/support.html#login). From a Linux or Mac system, open a terminal window and enter the following command (replacing `username` with your own username):

```
ssh username@stargate.cs.usfca.edu
```

This will log you into our gateway. However, Java is **not** installed on our gateway! You must next log into one of our lab computers. Enter `rusers` to find which systems are free. You want a system that has no users listed next to its name. Then, SSH into that lab computer. For example, if `g1201` is free, you can enter:

```
ssh g1201
```

You do not need to include your username or the domain "cs.usfca.edu" above, since you are already logged into a CS system.

See the [CS Support](http://www.cs.usfca.edu/support.html#login) guide for how to login using PuTTY if you have a Windows system.

## Getting Help

Your CS account is created and managed by our [CS Support](http://cs.usfca.edu/support.html) team. If you run into any issues with your account, please contact them via email at <support@cs.usfca.edu> or stop by Harney 536.

The instructor **cannot** reset your password for you, but we do have a test account you can use temporarily if you are having trouble during class.
