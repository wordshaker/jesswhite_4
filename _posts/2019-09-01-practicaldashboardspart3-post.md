---
layout: post
title: A Practical Guide To Dashboarding Part Three
description: "Metrics for APIs"
date: 2019-06-15
cover: "/assets/img/2019-09-01/traffic.png"
tags: [monitoring, instrumentation, dashboard]
comments: false
share: true
---

----
<center>
<h3> Baselines for APIs. </h3>
</center>

---
<br/>

As mentioned in the [previous post](https://jesswhite.co.uk/2019/04/15/practicaldashboardspart1-post.html) having baselines for dashboards can be useful for a variety of reasons.

* Recognising patterns for where to investigate when something goes wrong in your system.
* Transferrable knowledge across teams.

In this post, we shall explore how this applies to metrics measuring the health of APIs.

## Two Recommended Baselines
---

In this blog I am going to go through two main patterns for baselines of metrics for APIs.

- The Google Four Golden Signals
- R.E.D 

There is a lot of overlap between these patterns, and personally, I've used a mix of the two. There is a lot of literature around both, which agree on the strength of having baselines around API metrics. 

## [Googles Four Golden Signals](https://landing.google.com/sre/sre-book/chapters/monitoring-distributed-systems/)

---

The Four Golden Signals are mentioned in the Monitoring Distributed Systems chapter of the Google SRE book. Used in combination, the four metrics discussed are incredibly powerful.

### Latency 

This is the time between request and response but with a focus of the difference between successful and erroring requests. The reason for this is a slow error can give different context to a fast error, and it is always useful to know if a successful response is made within the expected time range. 

The example given in the SRE book is as follows

>  _For example, an HTTP 500 error triggered due to loss of connection to a database or other critical backend might be served very quickly; however, as an HTTP 500 error indicates a failed request, factoring 500s into your overall latency might result in misleading calculations_

Alongside helping to diagnose problems with the API, measuring API latency is also important for determining if the API is meeting any Service Level Agreements that have been agreed internally or externally. As you would have expected baselines around latency, you could even set alerts if your 95th percentile doesn't meet these expectations.

### Traffic 

This refers to the requests made to an API per second. The reason to measure this is to observe the load on the API and it's effects. If there is a spike in traffic that correlates with a problematic rise in latency or errors, it suggests that the API may want to be scaled to cope with the traffic. 

If the traffic is at expected levels, and there are problems elsewhere, it may not be dealing with the load that's causing your problems.

<div style="text-align:center; width:70%; margin-left: 10%;" markdown="1">
<img src="{{site.baseurl}}/assets/img/2019-09-01/traffic.png" alt="Errors">
</div>

---
_Analogy: In the picture, the latency is represented by how many cars cross the finish line in a set amount of times._

---

### Errors
same as before, a count of errors.

<div style="text-align:center; width:70%; margin-left: 10%;" markdown="1">
<img src="{{site.baseurl}}/assets/img/2019-09-01/error.png" alt="Errors">
</div>

---
_Analogy: There's no analogy here. An error is an error. It's just an excuse to draw Clippy._

---

### Saturation 
what percentage of your systems resources is currently in use.


## [R.E.D](https://peter.bourgon.org/blog/2016/02/07/logging-v-instrumentation.html)

---

RED, which is discussed in this blog written by [Peter Bourgon](https://peter.bourgon.org/blog/2016/02/07/logging-v-instrumentation.html), is a mnemonic coined by Tom Wilkie. Much like Brendan's Gregg USE methods for measuring system resources and services, RED is suggested as baseline measurements for API's.

### Rate
- a count of requests over time

### Error
- a count of error over time

### Duration 
- the time between request and response.



## Summary
---
 

---

_Chapter 2 - A Practical Guide To Dashboarding Series_

* <a href="{{site.baseurl}}/2019/04/15/practicaldashboardspart1-post.html">Part 1 - Introduction To Baselines for Dashboards</a>

* <a href="{{site.baseurl}}/2019/05/15/practicaldashboardspart2-post.html">Part 2 - Baselines for Services. </a>

* <strong><a href="{{site.baseurl}}/2019/09/01/practicaldashboardspart3-post.html">Part 3 - Baselines for API's.</a></strong>

---


_Chapter 1 - Creating & Maintaining Impactful Dashboards Series_

* <a href="{{site.baseurl}}/2018/04/09/impactfuldashboardspart1-post.html">Part 1 - Creation of impactful dashboards</a>

* <a href="{{site.baseurl}}/2018/04/22/impactfuldashboardspart2-post.html">Part 2 - Continuous Maintenance.</a>

* <a href="{{site.baseurl}}/2018/04/23/impactfuldashboardspart3-post.html">Part 3 - Danger Signs and Don'ts.</a>

---

<div style="text-align:center; width:20%; margin-left: 10%;" markdown="1">
<img src="{{site.baseurl}}/assets/img/logo.png" alt="Logo">
</div>
