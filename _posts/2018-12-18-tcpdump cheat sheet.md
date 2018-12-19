---
layout: post
title:  "Tcpdump cheat sheet"
date:   2018-12-18
author: David Xiao
categories: network tcpdump
tags:  network tcpdump
---

Listen on loopback for tcp traffic on port 4000. This is useful when you are debugging something purely local. Please be advised that the following command works for mac os, if you are using other OS, you may need to change the name of the interface `lo0`.

`tcpdump -i lo0 tcp port 4000 -w test.pcap`

For reading and analyzing .pcap file, I recommend Wireshark.


