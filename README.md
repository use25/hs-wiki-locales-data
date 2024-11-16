# hs-wiki-locales-data

This repository contains configs and other kinds of data to work with [Hearthstone Wiki](https://hearthstone.wiki.gg) localization project.

## How it works

* The main team (English team) will use ``locales.json`` as config for their tools, which pushes the Hearthstone data to the localized wikis with the matched locale data (such as text, name, strings and logos). This file consists of:
  * ``code``: an enum, also served as main ID and entries for other Hearthstone projects, such as [HearthSim's ``hsdata``](https://github.com/HearthSim/hsdata)
  * ``locIndex``: index number of the locale based on ``locValues`` arrays shown in ``samples.json``
  * ``wikiLink``: Localized wiki's domain name with ``https://``. Most of them should be ``https://hearthstone.wiki.gg/<WikiGG's locale code>``
  * ``uiName``: The name displayed for future GUI applications, which provide extra editing tools to help you manage your Wikis.
* You are free to contribute this repository as you wish. However:
  * Do not remove any key in ``locales.json``. This may result in the main team's tools being unable to function properly.
  * Please check if ``code`` and ``locIndex`` are matched with your wiki's localization and correct them.
  * You are free to add extra samples data to ``samples.json``, but do not arbuptly change the order of ``locValues``. Their values are already ordered in a way Hearthstone client is currently handling, not us.
* You can contact to the main team by the following to gain permissions to commit ``hs-wiki-locales-data``, as long as you are one of the admins in any localized wiki:
  * Create new section in [Hearthstone Wiki:Admin noticeboard](https://hearthstone.wiki.gg/wiki/Hearthstone_Wiki:Admin_noticeboard)
  * Create new section in Talk page of one of these users: [Hearthstone Wiki Administrators](https://hearthstone.wiki.gg/wiki/Hearthstone_Wiki:Administrators)
  * Posting message in any channel in [Hearthstone Wiki Discord server](https://discord.gg/pJCYXfuaDs)
  * Sending email to hearthstonewikiofficial@gmail.com
  * We also have accounts for other social media, but it's unlikely that we use them as main contacts