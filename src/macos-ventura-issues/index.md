---
layout: page
title: macOS 13 Ventura Issues
---

Since I've been using macOS Ventura, I've run into quite a few problems that I figured it'd be best to document on my website and see if anyone else had any they'd like to add.

If you've run into an issue not listed here, please email me directly at [slade@sladewatkins.com](mailto:slade@sladewatkins.com) or [submit a pull request](https://www.sladewatkins.com/docs/website/contributing/). (If you're emailing me for *any other reason*, please [go here](https://www.sladewatkins.com/contact/) first.)

---

## How to read
Items are written in the following format: 

```
[Version encountered in, Application/function affected] "Description of issue"
```

A source is also included if it wasn't encountered directly by me.

---

## Table of Contents
1. [Encountered](#encountered)
	- [System Settings](#system-settings)
	- [Mail](#mail)
2. [Resolved](#resolved)
	- [In macOS 13.3 Ventura](#in-macos-133-ventura)
	- [In macOS 13.2.1 Ventura](#in-macos-1321-ventura)
	- [In macOS 13.2 Ventura](#in-macos-132-ventura)
	- [In macOS 13.1 Ventura](#in-macos-131-ventura)
3. [From other folks on the internet](#from-other-folks-on-the-internet)

## Encountered
These are arranged by application or function, and I (Slade) encountered  them on a [2022 M2 MacBook Pro](https://support.apple.com/kb/SP870?locale=en_US) running macOS 13 Ventura.

###  System Settings
*__Author's note__: System Preferences was already bad, but it was stable. This is worse.*

- [13.1] System Settings is unreliable, as it locks up and crashes frequently.
- [13.1] System Settings doesn't display available updates, despite them being available.
- [13.1] Constant notifications regarding "new login items" despite nothing on my system actually changing.
- [13.1] Settings that were once easily accessible in the previous System Preferences are now gone, or harder to access, in the new System Settings app.
- [13.1] Searching for something doesn't work 95% of the time.

### Mail
*__Author's note__: Yes, I prefer macOS Mail, has never done anything wrong... except...*

- [13.1] Slow and unreliable at times, especially when moving a bulk amount of messages to another Mailbox or the Trash.
- [13.1] Freezes when reading emails from other Mailboxes other than the Inbox.

## Resolved

### In macOS 13.3 Ventura
- None

### In macOS 13.2.1 Ventura
- [13.2, Finder] Finder can't seem to remember that I have the Desktop folder favorited and regularly removes it from the Favorites list.
- [13.2, System Settings] AppleCare+ message won't go away despite declining it several times.

### In macOS 13.2 Ventura
- [13.1, Mail] I'm no longer seeing Mail get stuck downloading new messages and requiring a restart of any kind. Your mileage may vary. (Source is self)
- [13.1, System Settings] The third party widget configuration bug has been fixed, apparently. I didn't run into this, but many had. ([Source](https://blog.eternalstorms.at/2022/11/10/psa-macos-ventura-3rd-party-widget-configuration-broken/))

### In macOS 13.1 Ventura
- [13.0, System Settings] Network Locations has returned. ([Source](https://mjtsai.com/blog/2022/12/13/macos-13-1/))

## From other folks on the internet
- [Michael Tsai](https://mjtsai.com/blog/2022/12/27/ventura-issues/)
- [The Eclectic Light Company](https://eclecticlight.co/2022/11/04/fixes-and-flaws-in-ventura-13-0/)
