CensorTracker: Bypass Censorship
================================

[![Logo](/.github/media/censortracker_popup_en.png)](https://github.com/roskomsvoboda/censortracker)

![Build](https://github.com/roskomsvoboda/censortracker/workflows/Build/badge.svg?branch=master)
[![CodeFactor](https://www.codefactor.io/repository/github/roskomsvoboda/censortracker/badge)](https://www.codefactor.io/repository/github/roskomsvoboda/censortracker)

**CensorTracker** is a censorship circumvention extension for [Google Chrome] and [Mozilla Firefox].

[<img src="/.github/media/chrome-web-store.png" title="Chrome Web Store" width="170" height="48" />](https://chrome.google.com/webstore/detail/censor-tracker/gaidoampbkcknofoejhnhbhbhhifgdop)
[<img src="/.github/media/firefox-add-ons.png" title="Firefox Add-ons" width="170" height="48" />](https://addons.mozilla.org/ru/firefox/addon/censor-tracker/)

Features
========

CensorTracker provides a lot of useful features, here are the most
important:

- Configurable proxy
- Country-specific proxying
- Custom proxying list
- Bypass censorship and restrictions (including [DPI]-filtration)
- Warns about sites that transfer data to third parties

Development
===========

Prerequisites
-------------

Make sure you have required versions of `node` and `npm`, which are:

- `node v15.4.0` or higher
- `npm 7.6.3` or higher

Optionally, you may like:

- [`nvm`](https://github.com/nvm-sh/nvm)


The build was tested only on the following operating systems:

- `Ubuntu 19.10`
- `macOS Catalina v10.15.7`

We don't guarantee that CensorTracker will work on outdated versions of browsers,
so make sure you're using the latest ones.

We've tested CensorTracker on the following versions:

- Mozilla Firefox 80 or higher
- Google Chrome 80 or higher

Installation
------------

Firstly, you will need to install dependencies:

    ~ npm install


Now you can build an extension for Chrome like this:

    ~ npm run build:chrome
    ~ cd dist/chrome

and for Firefox, like this:

    ~ npm run build:firefox
    ~ cd dist/firefox


**Troubleshooting**: If you're getting error on building an extension using `npm`, please make sure that your
shell supports per-command environment variables (i.e something like this `NODE_ENV=production npm run build:firefox:prod`)


Going to production
-------------------

You can build a production version of the extension for Chrome like this:

    ~ npm run build:chrome:prod
    ~ npm run release:chrome
    ~ cd release/chrome

and for Firefox like this:

    ~ npm run build:firefox:prod
    ~ npm run release:firefox
    ~ cd release/firefox

License
=======

Censor Tracker is licensed under the MIT License. See [LICENSE] for more
information.

  [DPI]: https://en.wikipedia.org/wiki/Deep_packet_inspection
  [LICENSE]: https://github.com/roskomsvoboda/censortracker/blob/master/LICENSE
  [Google Chrome]: https://www.google.com/chrome/
  [Mozilla Firefox]: https://www.mozilla.org/en-US/firefox/new/
