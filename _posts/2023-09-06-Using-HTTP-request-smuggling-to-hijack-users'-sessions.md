---
title: Using HTTP request smuggling to hijack users' sessions
date: 2023-09-06
categories: [Write-up]
tags: [outpost24, exploit development]
image: ../assets/http-request-smuggling-hijack-preview.png
---

[Write-up](https://outpost24.com/blog/http-request-smuggling-to-hijack-user-session/)

In this blog (linked above) I walkthrough one of the most complex exploits I have created to-date resulting in application-wide session hijacking via HTTP Request Smuggling. The exploit abused [response queue poisoning](https://portswigger.net/web-security/request-smuggling/advanced/response-queue-poisoning#:~:text=Response%20queue%20poisoning%20is%20a,end%20to%20the%20wrong%20requests.) to desynchronize the application's response queue, and a small reflection gadget on the login page to eventually allow us to capture other users' **requests** including (of course) their session cookies.