---
title: "CRLF-Powered Desync Attacks: Beheading HTTP Streams"
date: 2026-05-20
categories: []
tags: [research]
image: /assets/BHUSA2026.webp
---

Coming to BlackHat USA 2026...


[Abstract](https://blackhat.com/us-26/briefings/schedule/index.html#crlf-powered-desync-attacks-beheading-http-streams-51712)

Have you ever discovered a header injection vulnerability and settled for little more than an open redirect or XSS? In this Briefing, we will introduce a battle-tested "header injection" powered desync methodology, enabling you to perform HTTP request smuggling attacks against even strictly RFC-compliant proxy chains.

We will begin by explaining a well-known but overlooked CRLF injection primitive that produced HTTP Request Splitting inside the core infrastructure of a major CDN, resulting in the capture of live users' credentials across thousands of compromised applications.

Building upon this, we'll demonstrate how header injections can be used to exploit more traditional smuggling attack classes, even when no parser discrepancy exists. Finally, we'll reveal how you can shift previously non-compliant desync attacks into the browser, unlocking a plethora of novel exploitation opportunities even when keep-alive connections are not shared between users. The result is a slew of real-word case studies with impacts ranging from account takeovers via desync-enabled XSS gadgets to cache poisoning, response queue poisoning, access control bypasses, and in several cases the possibility of creating the ever-terrifying desync worm.

To complement our methodology and case studies, we'll share our research journey and release two open-source tools that introduce robust detection of header injections regardless of your proxy of choice.