---
layout: page
title: Website - Revision Testing
---

Testing your revisions is really important, as when you launch a test server, you'll know immediately if you broke something (and potentially what you broke, as well).

This guide is written for macOS and can be loosely applied to Linux as well. If you use Windows, you're on your own.

## Prerequisites
You'll need [Homebrew](https://brew.sh) installed *before going any further*. Once you've installed it, run the following command in Terminal:

```
gem install bridgetown -N
```

And you're set. Now you can...

## Get going for the first time
First, start by cloning the [sladewatkins/website](https://github.com/sladewatkins/website) repository from GitHub using ``git``. **Make sure you do this in the parent directory where you'd like the files to be stored.**

```
git clone https://github.com/sladewatkins/website.git
```

Then, use ``cd`` to enter the directory you just created.

```
cd website
```

Then, run the following command to start the internal server included with Bridgetown:

```
bin/bridgetown start
```

And you now have a replica of this website running at [localhost:4000](http://localhost:4000)