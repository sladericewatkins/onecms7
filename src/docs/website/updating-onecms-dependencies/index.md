---
layout: page
title: Website - Updating OneCMS dependencies
---

When updating dependencies, be sure **not** to run the following command:

```
bin/bridgetown webpack update
```

OneCMS releases ``7.1.11`` and ``7.0.30`` **deprecate** the ``webpack update`` command and instead use the following commmand to manage updates:

```
yarn upgrade
```

## What it does now
The following command...

```
bin/bridgetown webpack update
```

...reverts the webpack back to what was initially forked from Bridgetown (upstream) in 2022. Since OneCMS aims to have more up-to-date dependencies than upstream, it does not make sense to officially sanction this command for version upgrades.

All commits that utilize either of the commands (the deprecated ``bin/bridgetown webpack update`` or officially sanctioned ``yarn upgrade``)