---
weight: 4
title: "Web is hard, reARMSEC aka ARMSec 2020"
date: 2020-12-27T01:00:00+04:00
lastmod: 2020-12-27T01:00:00+04:00
draft: false
author: "Davwwwx"
authorLink: "/about"
description: ""
resources:
- name: "featured-image"
  src: "featured-image.png"

tags: ["web security", "bug bounties", "hackerone", "owasp", "top 10", "conferences"]
categories: ["Conferences"]

lightgallery: true
toc:
  enable: false
---


At this year's Armsec seventh annual information security conference - [reARMSEC](https://armsec.org), I made a small presentation ([Google slides](https://go.xss.am/armsec2020), [PDF version](https://go.xss.am/armsec2020.pdf)) on why the modern web is hard describing [HackerOne's top 10](https://www.hackerone.com/top-ten-vulnerabilities) most impactful and rewarded vulnerability types for 2020. As for the real-life examples of the bugs, I gathered reports mostly from [HackerOne's Hacktivity](https://hackerone.com/hacktivity).
<!--more-->


XSS (Cache Poisoning): 
- [HackerOne report #394016, XSS on Discourse](https://hackerone.com/reports/394016) by [Sergey Bobrov](https://twitter.com/black2fan)
- [HackerOne report #415168, XSS on QIWI](https://hackerone.com/reports/415168) by [Sergey Bobrov](https://twitter.com/black2fan)

XSS (DOM):
- [XSS on Google Search (closure), mXSS](https://www.youtube.com/watch?v=lG7U3fuNw3A) by [Masato Kinugawa](https://twitter.com/kinugawamasato)
- [serialization bug in &lt;noscript&gt;](https://bugs.chromium.org/p/chromium/issues/detail?id=1160635) by [Michał Bentkowski](https://twitter.com/securitymb)
- [HackerOne report #876148, DOM XSS on DuckDuckGo](https://hackerone.com/reports/876148) by [Predrag Cujanović](https://twitter.com/cujanovic)

uXSS:
- [Semi Universal XSS affecting Firefox for iOS, CVE-2019-17004](https://0x65.dev/blog/2020-03-30/cve-2019-17004-semi-universal-xss-affecting-firefox-for-ios.html) by [Cliqz](https://twitter.com/cliqz)
- [uXSS in Chrome on iOS, CVE-2018-6128](https://bugs.chromium.org/p/chromium/issues/detail?id=841105) by [Tomasz Bojarski](https://bughunter.withgoogle.com/embed/profile/c25fa487-a4df-4e2e-b877-4d31d8964b82)

Electron:
- [Microsoft Teams zero click xss](https://github.com/oskarsve/ms-teams-rce/blob/main/README.md) by [Oskars Vegeris](https://www.linkedin.com/in/oskars-vegeris-b9b283125/)
- [Discord RCE](https://mksben.l0.cm/2020/10/discord-desktop-rce.html) by [Masato Kinugawa](https://twitter.com/kinugawamasato) (not in slides, but definitely a must read)

AAA vulnerabilities:
- [Exploiting e-mail systems](https://drive.google.com/file/d/1iKL6wbp3yYwOmxEtAg1jEmuOf8RM8ty9/view) by [Inti De Ceukelaire](https://twitter.com/securinti)
- [HackerOne report #493324, privilege escalation to gitlab admin](https://hackerone.com/reports/493324) by [Anton Subbotin](https://twitter.com/ska_vans)
- [Facebook Access Token Security Breach (30 million accounts)](https://about.fb.com/news/2018/09/security-update/) by :ghost:
- [HackerOne report #605720, vertical privilege escalation on HackerOne](https://hackerone.com/reports/605720) by [Vladimir Metnew](https://twitter.com/vladimir_metnew)
- [HackerOne report #663431, IDOR on HackerOne](https://hackerone.com/reports/663431) by [Jobert Abma](https://twitter.com/jobertabma)
- [Facebook account takeover via recovery code bruteforce](https://www.youtube.com/watch?v=U3Of-jF1nWo) by [Anand Prakash](https://twitter.com/sehacure)

Information Disclosure:
- [HackerOne report #396467, Snapchat's github token leaked publicly](https://hackerone.com/reports/396467) by [Majd](https://twitter.com/th3g3nt3lman)
- [HackerOne report #885539, Twitter private list members disclosure via GraphQL](https://hackerone.com/reports/885539) by [RyotaK](https://twitter.com/ryotkak)
- [HackerOne report #489146, confidential data of users and limited metadata of programs and reports accessible via GraphQL on HackerOne](https://hackerone.com/reports/489146) by [Yash Sodha](https://twitter.com/y_sodha) (not in slides, but definitely a must read)

SSRF:
- [HackerOne report #347139, LFI and SSRF via XXE on Rockstar Games](https://hackerone.com/reports/347139) by [Alex Birsan](https://twitter.com/alxbrsn)
- [HackerOne report #923132, redirect SSRF on Dropbox](https://hackerone.com/reports/923132) by [Sayaan Alam](https://twitter.com/ehsayaan)
- [HackerOne report #541169, SSRF via DNS rebinding on Gitlab](https://hackerone.com/reports/541169) by [Alex Chapman](https://twitter.com/ajxchapman)
- [HackerOne report #530974, Server-Side Request Forgery using Javascript on Snapchat](https://hackerone.com/reports/530974) by [Ben Sadeghipour](https://twitter.com/nahamsec)

CSRF:
- [HackerOne report #1010522, TikTok Careers Portal Account Takeover via CSRF](https://hackerone.com/reports/1010522) by [Lauritz](https://twitter.com/_lauritz_)

SSTI:
- [HackerOne report #125980, RCE via Flask Jinja2 Template Injection on Uber](https://hackerone.com/reports/125980) by [Orange Tsai](https://twitter.com/orange_8361)

Insecure Deserialization:
- [RCE on Facebook](https://devco.re/blog/2020/09/12/how-I-hacked-Facebook-again-unauthenticated-RCE-on-MobileIron-MDM-en/) by [Orange Tsai](https://twitter.com/orange_8361)

SQL injection:
- [HackerOne report #137956, Error based SQL injection on Mail.ru](https://hackerone.com/reports/137956) by [Vahagn Israelian](https://twitter.com/0xKonqi)
- [HackerOne report #10037, Boolean based SQL injection on Mail.ru](https://hackerone.com/reports/10037) by [Vahagn Vardanian](https://twitter.com/vah_13)
- [HackerOne report #786044, Time based SQL injection on Mail.ru](https://hackerone.com/reports/786044) by [Austin Augie](https://twitter.com/area_fishing)
- [HackerOne report #852306, SQLI Wildcard Injection on Mail.ru](https://hackerone.com/reports/852306) by [Alexey (bazzy)](https://hackerone.com/bazzy)


To learn more (I'll try to update this list constantly):
- Books - [Web Application Hacker's Handbook](https://www.amazon.com/Web-Application-Hackers-Handbook-Exploiting/dp/1118026470), [Web Hacking 101](https://leanpub.com/web-hacking-101), [The Tangled Web](https://www.amazon.com/Tangled-Web-Securing-Modern-Applications/dp/1593273886), [The Art of Software Security Assessment](https://www.amazon.com/Art-Software-Security-Assessment-Vulnerabilities/dp/0321444426)
- Writeups - [HackerOne's Hacktivity](https://hackerone.com/hacktivity), [bugcrowd's CrowdStream](https://bugcrowd.com/crowdstream), [CTFtime.org writeups](https://ctftime.org/writeups)
- Labs - [PortSwigger Web Security Academy](https://portswigger.net/web-security), [TryHackMe](https://tryhackme.com/), [hackxor](https://hackxor.net/), [OverTheWire: Wargames](https://overthewire.org/wargames/)

Follow these people/pages - [https://twitter.com/davwwwx/following](https://twitter.com/davwwwx/following)
