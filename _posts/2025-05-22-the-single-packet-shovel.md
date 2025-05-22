---
title: "The Single-Packet Shovel: Digging for Desync-Powered Request Tunnelling"
date: 2025-05-22
categories: [Research]
tags: [assured, bug-bounty]
image: ../assets/shovels.webp
---

[Research](https://www.assured.se/posts/the-single-packet-shovel-desync-powered-request-tunnelling)

[Recording]()

Despite HTTP Request Tunnelling's resurgence in recent years with the advent of HTTP/2 Desync Attacks, its much bolder big brother HTTP Request Smuggling has stolen the limelight, leaving cases of desync-powered tunnelling buried for all but the most dedicated tunnelling enthusiasts.

In this paper I will reveal the discovery of wide-spread cases of request tunnelling in applications powered by popular servers including IIS, Azure Front Door and AWS' Application Load Balancer including the creation of a novel detection technique that combined the recently popularized "Single-Packet Attack" with our ever-trusty HTTP desync techniques.

Throughout the journey I will also explore the complexities of navigating security research for the first time, drawing parallels from the advice given in so you want to be a web security researcher and illuminate the ease through which existing tooling from industry leading researchers can be adapted in order to rapidly test your own ideas, even with a rudimentary understanding of programming.

This research was originally presented at BSides Exeter 2025 the recording for which will be released soon.