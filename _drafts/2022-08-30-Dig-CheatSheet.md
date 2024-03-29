---
layout: single
title:  "Dig CheatSheet"
categories: Computing Homelab
publish: false
---

## Being Selective

You don’t have to settle for the two extremes of tight-lipped and garrulous. The dig command allows you to selectively include or exclude sections from the results.

The following query options will remove that section from the results:

* +nocomments: Don’t show comment lines.
* +noauthority: Don’t show the authority section.
* +noadditional: Don’t show the additional section.
* +nostats: Don’t show the stats section.
* +noanswer: Don’t show the answer section.
* +noall: Don’t show anything!

The +noall query option is usually combined with one of those above to include a section in the results. So, instead of typing a long string of query options to turn off multiple sections, you can use +noall to turn them all off.

You can then use the following inclusive query options to turn those you want to see back on:

* +comments: Show comment lines.
* +authority: Show the authority section.
* +additional: Show the additional section.
* +stats: Show the stats section.
* +answer: Show the answer section.
* +all: Show everything.

## Reference

* [Hostinger Tutorials](https://www.hostinger.co.uk/tutorials/how-to-use-the-dig-command-in-linux/) a well written set of tutorial on dig and instructions on how to install it on Linux.
* [NixCraft](https://www.cyberciti.biz/faq/linux-unix-dig-command-examples-usage-syntax/) - Unix and Linux dig command examples
* HowtoGeek - How to use the [Dig Command](https://www.howtogeek.com/663056/how-to-use-the-dig-command-on-linux/)
* The [Linux Handbook](https://linuxhandbook.com/dig-command/) on Dig Command on Linux Explained.
* DYN [How to use BIND’s Domain Information Groper (dig) Tool](https://help.dyn.com/how-to-use-binds-dig-tool/)
