# SladeWatkins.com
[![CLA assistant](https://cla-assistant.io/readme/badge/sladewatkins/website)](https://cla-assistant.io/sladewatkins/website) [![Deploy to Prod](https://github.com/sladewatkins/website/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/sladewatkins/website/actions/workflows/gh-pages.yml)

This is the source code for SladeWatkins.com, it's largely what makes my website tick. It's built on top of [Bridgetown](https://github.com/bridgetownrb/bridgetown) and mostly follows upstream, though has a couple tweaks specific to the environments I run it in.

The tweaks and changes from Bridgetown 1.1.0 include:
- custom integrations with local CI... self explanatory.
- support for Ruby 3.1.y out of the box.
- more up-to-date dependencies and assets than Bridgetown (upstream).
- Netlify/DigitalOcean deployment integration (this is proprietary, for now, while the code is worked out). *Right now, this repository uses the gh-pages related action to send the output to the correct tree, then the CI checks out the latest prod-x-y (x being the date, and y being the time) tag, and uploads that to Netlify/DigitalOcean.*
- Additionally, the versioning follows that of OneCMS. Prior to version 6, OneCMS was a proprietary content management system I had developed for use with several of my projects in 2020, then again in 2021-2022. It has since been replaced by version 7+, which is an open-source fork of [Bridgetown](https://github.com/bridgetownrb/bridgetown) and contained within *this very repository*.
	- **Compatibility**: Since OneCMS 7+ is a fork of Bridgetown, it is compatible with all of its plugins and other add-ons. It is also able to rebased on to the latest versions of the upstream repository.

## Licensing
I've open sourced OneCMS 7+ under the [MIT License](https://github.com/sladewatkins/website/blob/master/LICENSE-MIT). (Do note that my blog and site text are licensed under the [CC-BY-SA-4.0 license](https://github.com/sladewatkins/website/blob/master/LICENSE-CC-BY-SA-4.0).)

## Production assets
The [``gh-pages``](https://github.com/sladewatkins/website/tree/gh-pages) tree within this repository contains the production assets served to the public on [sladewatkins.com](https://www.sladewatkins.com).

## About this site
I'm building this site to be database-free, no SQL of any kind to be found. I hate working with SQL (and maintaining those servers) and this is my attempt to stop doing so.

TL:DR: this simply requires a webserver, as well as support for Ruby and [Bridgetown](https://www.bridgetownrb.com/) (if hosting locally for development), and it DOESN'T REQUIRE SQL/Database servers of any kind. Yay!

## The [``staging``](https://github.com/sladewatkins/website/tree/staging) branch
The [``staging``](https://github.com/sladewatkins/website/tree/staging) branch is special - that's where all commits set to roll out to production ("master" branch) need to sit and be tested by Slade's Continous Integration (CI) system + a few of his physical systems. This is to ensure no issues are found and things keep going smoothly.

## Find an issue?
If you find an issue, you might be able to patch it up yourself! Check out [the guide](https://www.sladewatkins.com/docs/website/) to see how you can help. When you've put together your changes, submit them as a [pull request](https://github.com/sladewatkins/website/pulls) directed to the [``staging``](https://github.com/sladewatkins/website/tree/staging) branch! I'll take a look at it and might merge it in. (Note: all PRs sent to the ``master`` branch won't be considered. Commits must target ``staging``, see [the documentation here](https://www.sladewatkins.com/docs/website/how-staging-works/) for more details.)

If you'd prefer to just report it, please do so using the [issues tab](https://github.com/sladewatkins/website/issues).

## Report security issues (live site)
Though, for security issues relating to the server I use on sladewatkins.com directly, I ask you [reach out privately](https://www.sladewatkins.com/contact/).
