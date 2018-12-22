---
layout: post
title:  "Tcpdump cheat sheet"
date:   2018-12-18
author: David Xiao
categories: network tcpdump
tags:  network tcpdump
---

### Monitor on loopback interface for tcp traffic on port 4000

This is useful when you are debugging something local. The following sample command works for mac os, if you are using other OS, you may need to change the `-i lo0` portion.

`tcpdump -i lo0 port 4000 -w test.pcap`

Then you can use wireshark to read and analyze the .pcap file.

