---
layout: post
title:  "They don't make config files like they used to"
date:   2017-05-31 21:25:00 +0000
---

I was having a think about configuration file formats the other day and it occurred to me that so-called legacy configuration file formats could be better than
the formats we currently use.

Configuration files are read by applications but maintained by human beings. (I'm not including configurations which are maintained by a GUI administration
application. In those circumstances you'll never open the file directly as you'll always use the tool.) Therefore, in my opinion, the file format should be
optimised for people: It should be easy for them to understand and to update manually. All a computer needs to do is be able to read in and parse the file.

Most configuration files just contain a list of key/value pairs. **So.. Simple huh?**

Back in MS-DOS and early versions of Windows, [INI files](https://en.wikipedia.org/wiki/INI_file) were a very common standard. They generally just held one
setting per line such as: **SOURCEDIR=C:\Source**

I'm not sure why INI files got less popular? Maybe it was because we started loading settings into the [Windows Registry](https://en.wikipedia.org/wiki/Windows_Registry).
I think with hindsight most of us probably agree that the Registry is not a great place to store general application settings outside of low-level operating system
options. It became a bucket for everything and recklessly editing the Registry (and getting it wrong) could have some fairly harsh system stability consequences.

After that, I think [XML](https://en.wikipedia.org/wiki/XML) became popular. You could store anything you liked in an XML file.. So we stored **EVERYTHING** in XML!
Especially configuration files. The problem with XML is that it contains a lot of "noise". Schema declarations, opening tags, crazy amounts of attributes, closing tags.
Generally stuff that is part of the file format but isn't your configuration data. Additionally, if your actual configuration values contained angle brackets or ampersands
you would need to escape them out. Nasty!

Currently we seem to be in love with [JSON](https://en.wikipedia.org/wiki/JSON). It's probably an improvement over XML but is it *really* a good format for
human-readable data? Nevertheless, it has widespread adoption as a configuration file format. Just be careful you remember trailing commas and put curly and square
braces in all the right places. Not to mention ensuring you keep the indentation neat to retain some level of readability.

**So where do we go from here?**

Personally, I'm becoming of fan of [TOML](https://en.wikipedia.org/wiki/TOML) which stands for "Tom's Obvious, Minimal Language". It's not currently a standard
and is still being defined. But, it's clean and very much like an evolved version of the INI format.
