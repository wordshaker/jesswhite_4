---
layout: post
title: "Error! Error!"
description: "Getting your error levels right - An assessment of error levels and what they mean"
date: 2017-03-11
tags: [article, monitoring, alerting, errors]
comments: true
share: true
---

# Error! Error!

We are going to explore different levels of error, what they mean and when they should be used.
I'm currently using these levels in C# using Serilog, so this is where they will probably most applicable
but the concepts will be made as generic as possible.

## Basic Error levels

There are many different levels available for logging including:

```
1. FATAL
2. ERROR
3. WARN
4. INFO
5. DEBUG
6. TRACE 
7. VERBOSE
```

But what do these mean and when should you use them? For consistent and effective logging this is something that should be agreed on.

#### FATAL

THE WORLD IS ENDING! This is for the worst of the very worst situation. This is for situations which force the application to close.
As such their use should be very rare, if used at all. 

<div style="align:center; width:300px; height:300px; margin-left: 30%;" markdown="1">
![Fatal](/assets/images/2017-03-11/fatal.gif)
</div>

#### ERROR

This is for something that has gone wrong that will not close force the application to close but it will cause issues. It is for those 
problems that require immediate intervention.


#### WARN

This is for problems that do not require immediate intervention, but that may cause issues at some point or peculiarities. It provide information
but it isn't something to act upon. The application continues even if it's full behaviour isn't quite as expected.

Personally, I wouldn't use this level of logging, as if it's not actionable, in my opinion people won't pay attention to it. Why not throw an error 
where it would be a problem instead, or if possible, guard against the possibility of their being an issue. 

It is used however. An example given in [2] is for logging bad login attempts for example. This could be used to assess problems in user exeperience.
Something to consider is there are other tools that could be used for this purpose effectively.

#### INFO




#### DEBUG



#### VERBOSE


### In conclusion..

As mentioned throughout, how to use logging levels is not something that is completely concrete. In this article, I have explored my interpretation of
what the levels mean and how to use them. This is from how I would use them in my job as a developer, but also from reading other peoples useage. Please send me any 
resources on the topic, or experiences that you have found useful.

<div style="align:center; width:300px; height:300px; margin-left: 30%;" markdown="1">
![End](/assets/images/2017-03-11/end.gif)
</div>

### References 

1. [https://dave.cheney.net/2015/11/05/lets-talk-about-logging](Lets Talk About Logging - Dave Cheney)
2. [http://stackoverflow.com/questions/2031163/when-to-use-the-different-log-levels](StackOverflow - Logging Levels)