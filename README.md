# SladeWatkins.com
[![CLA assistant](https://cla-assistant.io/readme/badge/sladewatkins/onecms7)](https://cla-assistant.io/sladewatkins/onecms7) [![Deploy to Prod](https://github.com/sladewatkins/onecms7/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/sladewatkins/onecms7/actions/workflows/gh-pages.yml)

This is the source code for SladeWatkins.com, it's largely what makes my website tick. It's built on top of [Bridgetown](https://github.com/bridgetownrb/bridgetown) and mostly follows upstream, though has a couple tweaks specific to the environments I run it in.

## Differences between OneCMS and Bridgetown
The tweaks and changes from Bridgetown include:
- custom integrations with local CI... self explanatory.
- support for Ruby 3.1.y out of the box.
- more up-to-date dependencies and assets than Bridgetown (upstream).
- Netlify/DigitalOcean deployment integration (this is proprietary, for now, while the code is worked out). *Right now, this repository uses the gh-pages related action to send the output to the correct tree, then the CI checks out the latest prod-x-y (x being the date, and y being the time) tag, and uploads that to Netlify/DigitalOcean.*
- Additionally, the versioning follows that of OneCMS. Prior to version 6, OneCMS was a proprietary content management system I had developed for use with several of my projects in 2020, then again in 2021-2022. It has since been replaced by version 7+, which is an open-source fork of [Bridgetown](https://github.com/bridgetownrb/bridgetown) and contained within *this very repository*.
	- **Compatibility**: Since OneCMS 7+ is a fork of Bridgetown, it is mostly compatible with all of its plugins and other add-ons. It is also able to rebased on to the latest versions of the upstream repository.

## Licensing
I've open sourced OneCMS 7+ under the [MIT License](https://github.com/sladewatkins/onecms7/blob/master/LICENSE). (Do note that my blog and site text are licensed under the [CC-BY-SA-4.0 license](https://github.com/sladewatkins/onecms7/blob/master/LICENSE-CC-BY-SA-4.0).)

## About this site
I'm building this site to be database-free, no SQL of any kind to be found. I hate working with SQL (and maintaining those servers) and this is my attempt to stop doing so.

TL:DR: this simply requires a webserver, as well as support for Ruby and [Bridgetown](https://www.bridgetownrb.com/) (if hosting locally for development), and it DOESN'T REQUIRE SQL/Database servers of any kind. Yay!

### Production assets
The [``gh-pages``](https://github.com/sladewatkins/website/tree/gh-pages) tree within this repository contains the production assets served to the public on [sladewatkins.com](https://www.sladewatkins.com).

## Maintaining the codebase
OneCMS/Slade's website is maintained and updated regularly to ensure it is up-to-date, accurate, and of course: secure.

### The [``staging``](https://github.com/sladewatkins/onecms7/tree/staging) branch
The [``staging``](https://github.com/sladewatkins/onecms7/tree/staging) branch is special - that's where all commits set to roll out to the latest OneCMS release and production website ("master" branch) need to sit and be tested by Slade's Continous Integration (CI) system + a few of his physical systems. This is to ensure no issues are found and things keep going smoothly.

For documentation regarding how dependencies are upgraded within OneCMS/this repository, see [the documentation](https://www.sladewatkins.com/docs/website/updating-onecms-dependencies/).

### Version support
The two most recent point releases of OneCMS are supported and maintained, with the oldest supported release getting vital security updates **only**.

Currently supported/maintained releases:
- [7.2.y (current)](https://github.com/sladewatkins/onecms7/tree/master)
- [7.1.y](https://github.com/sladewatkins/onecms7/tree/version-7.1.y)

Versions prior to the above are End-Of-Life and are no longer supported. OneCMS 7.2 will lose support in April 2023, following the release of OneCMS 8.1.

### Mirrors
I mirror this repository on both [GitHub](https://github.com/sladewatkins/onecms7) and [Gitlab](https://gitlab.com/sladewatkins/onecms7). Both repositories the same codebase, refs, and other information as one another.

## Find an issue?
If you find an issue, you might be able to patch it up yourself! Check out [the guide](https://www.sladewatkins.com/docs/website/) to see how you can help. When you've put together your changes, submit them as a [pull request](https://github.com/sladewatkins/onecms7/pulls) directed to the [``staging``](https://github.com/sladewatkins/onecms7/tree/staging) branch! I'll take a look at it and might merge it in. (Note: all PRs sent to the ``master`` branch won't be considered. Commits must target ``staging``, see [the documentation here](https://www.sladewatkins.com/docs/website/how-staging-works/) for more details.)

In anticipation of the OneCMS 8.0 release in March, we are turning off issue reporting for OneCMS 7.1 and later. We will continue to maintain both versions in the meantime.

## Report security issues
Please see the [SECURITY.md](https://github.com/sladewatkins/onecms7/blob/master/SECURITY.md) file for more information on reporting security issues.