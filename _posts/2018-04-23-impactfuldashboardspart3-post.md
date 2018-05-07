---
layout: post
title: Creating & Maintaining Impactful Dashboards Part Three
description: "Danger Signs of Dashboarding"
date: 2018-04-23
img: ./2018-04-23/header.png
tags: [monitoring, instrumentation, dashboard]
comments: false
share: true
---

----
<center>
<h3> Danger Signs of Dashboarding - Times to make a change. </h3>
</center>
--- 
<br/>


We have covered what needs to be covered on a day-to-day aspect of working with dashboards. This series so far has explored the conversations in creation and maintenance of dashboards. What we haven't explored are the signs that a dashboard may need a bit of clearing up or re-work. Here we will go through a few of them, why they might happen and what to do when they do.

### "I don't know what the metrics are for"

_"I don't know what these metrics mean"_, _"Which dashboard should I be using"_, _"I don't know what the metrics are for"_...

All of these statements point to the same issue, and it's a very common problem. Monitoring isn't being treated like a first class citizen and the dashboards are stale, out of date, out of context and probably no longer useful. The systems and projects we work on and care about are ever evolving. We want them to grow and change, as it shows progress, but often monitoring, in particular dashboarding, gets left behind. 

Not knowing what your metrics mean or are for anymore is a symptom of numerous problems:

- _Stale / obsolete information_

    Your dashboards and other forms of monitoring aren't being updated with the systems / projects that they are monitoring. In terms of your dashboards, this can mean that some of the metrics shown are no longer measured or present or may be stable now.  All in all - your dashboards are crowded with metrics that should have been deprecated.

    This is a problem for numerous reasons. Firstly, how are you supposed to know which of the metrics displayed are useful to you or not? Especially as a newer person to the company that might be using the dashboards to aid them trace or debug (though log analytics are better for this purpose if available) this can be confusing.

    Secondly, we are supposed to be able to react to the metrics on our dashboards. There should be a purpose to them. you cannot react to stale or obsolete data. Also, if that is present it suggests the boards haven't been updated in a while and may be missing information you need to know about.

- _Problems with communication_ 
   
    The previous posts have had emphasis on the importance of communication when producing and maintaining dashboards. If the metrics have been put on this board without conversations being had about the purpose and audience of the board, what needs measuring and why, and how long it needs measuring for - you will be lucky to be making the most out of it. 

    Dashboards should always have a purpose and there should be a suitable reaction to the metrics displayed on a dashboard.

    This is even more of a issue if the person making the dashboard is separate from the work the dashboard is responsible for. If you aren't working on the system or project, it's unlikely you will know if the information is relevant or needs changing. I'll come back to this later.

- _Bad annotation_ 

    Dashboards should be clear. Whether its by using titles, panels or what ever feature you think is beneficial it should be possible for someone working in the area the dashboard is covering to look at it and work out what is what relatively quickly.

    If you can't do this clearly on the display - make sure that those who will need to be using the boards are trained on the stats that are displayed, what they mean, and what to do when it's gone Pete Tong.

- _"This might be interesting"_

    There are many things in life that are interesting. Unfortunately, these things aren't always useful and don't have a reaction that needs to be taken against them. 

    Dashboards are used to inform us of the current state of play. The metrics displayed on them should be things we can react to, even if it is to plan improvements to our systems. By adding information without a purpose for it, leads to busy, cluttered dashboards. This will include metrics which were once added out of interest, but nobody knows what they are for or what should be done with them.


#### What can I do?

The reason this is listed as a danger sign is that the dashboards are now not easy to read or understand, there is not a strong purpose to them and it is hard to react to the metrics. As they become harder to use, they become more of a hindrance than a help.

In my opinion, if a dashboard is in this state the only thing to do is to go back to basics. Delete the board. Have the necessary discussions to determine if anything needs to be monitored in relation to this are of the system or project. If there is, talk to the stakeholders / audience of the dashboard and start fresh.


### "Dashboards are a tick box exercise"


#### What can I do?



### "We have one person responsible for our dashboards"


#### What can I do?

### "Vanity Metrics"

### Busy Boards / Too many boards

### I Hate Pie



---

Creating & Maintaining Impactful Dashboards Series

Part 1 - [Creation of impactful dashboards](https://jesswhite.co.uk/impactfuldashboardspart1-post/)

Part 2 - [Continuous Maintenance.](https://jesswhite.co.uk/impactfuldashboardspart2-post/)

**Part 3 - [Danger Signs and Don'ts.](https://jesswhite.co.uk/impactfuldashboardspart2-post/)**

---