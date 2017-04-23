---
layout: post
title: "Hack Yourself First Day"
description: "An Oakbrook hack day to learn about security"
date: 2017-04-05
tags: [article]
comments: true
share: true
---

Our resident shady coder Jordan, organised an epic hack day at Oakbrook to teach us a thing or two about hacking and 
security. For the first half of the day we were given a list of tools we could investigate. These were both to hack and 
for helping to make apps more secure.

<div style="align:center; width:80%; margin-left: 8%;" markdown="1">
![Hack](/assets/images/2017-04-05/hacker.jpg)
</div>

The second half of the day, we played capture the flag. Jordan hosted two versions of [Troy Hunts](https://www.troyhunt.com/) [Hack Yourself First](https://hackyourselffirst.troyhunt.com/) website with a nifty scoreboard of vulnerabilities. We were split into 2 teams, and 
were awarded points for successful attacks and pre-emptive defence against certain attacks. 

This day wasn't just for fun. It was to open our eyes to many security issues we wouldn't otherwise have considered. But... IT 
WAS REALLY FUN!

# First Half

There were a couple of products I took time to investigate. Here is the overview of the opinions I had formed:

### [Acunetix](https://www.acunetix.com/blog/docs/acunetix-quick-start-guide/)

This was the first product I explored on the first half of the day, and I'm not ashamed to say I fell in love.
Acunetix is used to scan and detect vulnerabilities on a site. 

I only use the free version of this product - but was really impressed with its features. When conducting a scan 
any vulnerabilities found during its progress were displayed so that you don't have to wait for the final reports 
for the results. There are different levels of error, so it is clear which are urgent and which are a lower risk.

Another feature, which I found especially exciting, is that when a scan is complete there were a choice of reports that could 
be produced. an OWASP report, compliance level report, dev level report - these were but a few of the options. These are 
produced in a format that has information suitable for the needs of those who are going to receive it. For example, the dev 
report says the vulnerability, the level and guidance on where it could be found. 

**Pros:**
```
+ Nice UI
+ Real time feedback
+ Lots of scanning options
+ Different formats of reports can be produced
```

**Cons:**
```
- Scanning is pretty slow
```
### Others 

- [Cain & Abel](http://www.oxid.it/cain.html)
- [Harvester](https://github.com/laramies/theHarvester)
- [Metasploit](https://www.metasploit.com/)

Unfortunately, I couldn't test out any of the above. Between anti-viruses and firewalls
I couldn't even get a couple of them to download onto my machine.

# Capture The Flag

As explained in the introduction, we were split into two teams to play capture the flag.
Our team split into 3 parts:

- Attackers: attacked the site using tools such as [SQLmap](http://sqlmap.org/),
- Defenders: fixed vulnerabilities in the site. 
- Testers: Found weakness' in the teams site to fix, and the opposing teams site to attack.

I was a tester in this team, which gave me a good chance to put Acunetix to the test.

This game was great fun - and I really hope Jordan presents it at a meetup near you. His scoring
table was nifty. 

# Overview

This day was not just for entertainment but also for learning. It has certainly met that purpose. 
A lot of us felt that not only did we learn a lot on the day, but also learnt about how little we knew
 about the topic of security.

A lot of what we took from the day will go on to be applied in our site. It has definitely inspired others to 
do the [hack yourself Pluralsight course](https://www.pluralsight.com/courses/hack-yourself-first) to learn a bit more about this vast topic.

