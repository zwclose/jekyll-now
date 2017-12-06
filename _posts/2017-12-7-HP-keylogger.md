---
layout: post
title: HP keylogger
---

TL;DR:
HP had a keylogger in the keyboard driver. The keylogger saved scan codes to a WPP trace. The logging was disabled by default but could be enabled by setting a registry value (UAC required).
Get the list of affected hardware and patch here: https://support.hp.com/us-en/document/c05827409

***
Sometime ago someone asked me if I can figure out how to control HP's laptop keyboard backlit. I asked for the keyboard driver SynTP.sys, opened it in IDA and after some browsing noticed a few interesting strings:

![Strings](/_posts/Strings.PNG)
