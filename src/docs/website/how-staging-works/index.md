---
layout: page
title: Website - How staging works
---

Patches, pull requests, and anything from anyone are pulled into the ``staging`` branch (or "tree"). That tree is the destination for all in-progress work.

You can think of this as the destination for commits that are ready to get pushed to production, but on their own, are too insignificant to be pushed on their own. Once enough commits pile up in staging*, then (and only then) will I pull them up into the ``master`` tree. ``staging`` then effectively resets, both trees become equal, allowing me to pick back up from square one.

*Though, at the very least, I try to clear the ``staging`` tree at least once daily. That way things aren't getting _too_ clogged up.