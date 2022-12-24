---
layout: page
title: OneCMS Versioning
---

Here's how the versioning system works for OneCMS:
1. The numbering system is ``MAJOR.MINOR.PATCH``.
2. If the code contains minor updates to the base of OneCMS's generation system (which itself is based on Bridgetown), the ``PATCH`` number is updated by one.
3. If the code contains new pages or additions to the website, but no other updates to the generation system were made, no ``MAJOR``/``MINOR``/``PATCH`` numbers are updated: it is considered the same release.
4. If the code contains major updates to the base of the generation system, the ``MINOR`` number is updated by one, and ``PATCH`` number is reset.