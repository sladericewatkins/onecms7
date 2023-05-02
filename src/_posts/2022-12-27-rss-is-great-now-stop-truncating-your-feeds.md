---
layout: post
title:  "RSS is great, now stop truncating your feeds"
date:   2022-12-27 12:30:00 -0500
author:  Slade Watkins
categories: blog
---

[RSS](http://rssboard.org/rss-specification) (which is known fully as “Really Simple Syndication”) has been around for *a long time*. It’s a simple way to consume and enjoy content from all across the web, and many website owners (usually those with news sites or blogs) include a version of their website using the RSS standard for people who get their news from an RSS reader app.

Of course, that’s not the only thing RSS can do: it was used as the basis of [.svg](https://blog.hubspot.com/website/what-is-an-svg-file), and Tom Scott [uses it to promote his videos](https://www.tomscott.com/updates.xml). Unfortunately, I’ve noticed a serious problem with the standard, especially as I’ve started testing Reeder for the iPhone, iPad, and Mac (which uses RSS feeds to fetch content from across the web)…. And that is that **most RSS feeds are *almost always* truncated.**

Truncated means that the post available in the RSS feed is shortened significantly — directing users to their website to read the feed update instead of the RSS reader app they’re currently in. The reason why a website owner might do this is obvious — targeted, privacy-unfriendly ads are obviously a huge way for site owners to make a boat load of money *fast* — and RSS presents an obvious roadblock to that. 

Because RSS was designed to be “private” in the sense that it doesn’t grab in-line ads, doesn’t support the tracking of visit time or views, and — depending on the site owner — doesn’t always load in-line images either.

Now, there are some ways around this of course, though it would cost site owners a lot of money if they’re on some sort of [pay-per-click/view plan with their client](https://www.sladewatkins.com/blog/and-now-a-word-from-our-sponsor/). A couple examples I can think of include:
- Sponsored excerpts (insert these into posts); or
- Sponsored posts ([similar to how MacStories does it](https://www.macstories.net/sponsored/))

I believe in the open, but private web. I believe every site should be an interconnected web of information and utility, not plastered banner ads and [overwhelming interfaces that change weekly](https://twitter.com/Ark_shitposts/status/1606043352251527168). 

This means shifting away from proprietary, forced interfaces and finding new ways to adapt. You can see this in action with [ActivityPub](https://activitypub.rocks) and how a mass amount of users are [migrating from Twitter](https://metro.co.uk/2022/12/26/mastadon-gains-millions-of-new-users-as-twitter-exodus-continues-17997380/) to [Mastodon, a piece of open-source software](https://github.com/mastodon/mastodon) built on said standard.

So, stop truncating your RSS feeds. Open up the floodgates and let folks choose how they want to consume your content. (By the way: the RSS feed for my site is [here](https://www.sladewatkins.com/feed.xml)!)