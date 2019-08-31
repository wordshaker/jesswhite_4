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
the time between request and response but with a focus of the difference between successful and erroring requests.


### Traffic 
requests per second. A measure of the load on the API.

<div style="text-align:center; width:70%; margin-left: 10%;" markdown="1">
<img src="{{site.baseurl}}/assets/img/2019-09-01/traffic.png" alt="Errors">
</div>

---
_Analogy:ut._

---

### Errors
same as before, a count of errors.

<div style="text-align:center; width:70%; margin-left: 10%;" markdown="1">
<img src="{{site.baseurl}}/assets/img/2019-09-01/error.png" alt="Errors">
</div>

---
_Analogy:ut._

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
