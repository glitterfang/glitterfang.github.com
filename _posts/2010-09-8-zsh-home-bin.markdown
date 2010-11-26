---
layout: post
title: How To Get ~/bin In Your Path
description: The solution to the problem that I struggled with for months.  Sometimes you just don't know what to search for.
---

## [{{ page.title }}]({{ page.url }})

I want to show you how to get your ~/bin directory in your path using zsh.  I couldn't get this to work for months.  A few days ago, I finally did.  Here's how.

### The Issue
zsh doesn't expand the tilde character.

### The Fix
You can fix this problem with two solutions.

### The Quick Fix:
Just type in the complete path to the bin directory.  On OS X, 

`export PATH="/Users/x/bin."`

If you use your dotfiles on multiple machines with different operating systems, this complete path breaks.

### The Better Solution:
To be a good zsh practitioner, use the HOME environment variable.  This is set with the proper path to your home directory, no matter where you are.

`export PATH="$HOME/bin"`

I hope this helps someone.
