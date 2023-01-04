---
layout: page
title: Website - Revision Testing
---

Testing your revisions is really important, as when you launch a test server, you'll know immediately if you broke something (and potentially what you broke, as well).

This guide is written for macOS and can be loosely applied to Linux as well. If you use Windows, you're on your own.

## Prerequisites
You'll need [Homebrew](https://brew.sh) installed *before going any further*. Once you've installed it, you'll need to install ``node`` and ``yarn`` on your system.

You can do so by running:

```
brew install node
brew install yarn
```

Then, install ``bridgetown`` by running:
```
gem install bridgetown -N
```
*Don't worry, OneCMS runs on top of Bridgetown's upstream repository (for now) so you're all set. In the future, versioning may be handled by a separate gem.*

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

And you now have a replica of this website running at [localhost:4000](http://localhost:4000). Use this server to test your revisions.