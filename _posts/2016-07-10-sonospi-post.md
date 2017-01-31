---
layout: post
title: "Sonos Pi Project"
description: "For alerting on sonos based on datadog events"
date: 2016-07-10
tags: [project, js]
comments: true
share: true
---

## About
This was a joint project between myself and my partner Moreton as our first attempt at using a RaspberryPi and test driving a Node.JS project. We both wanted to learn node and when I came up with the project idea as a piece of fun to help out the place I work at; it seemed like the perfect opportunity to learn Node.

<div style="text-align:center; margin-left: 30%" markdown="1">
![Pi](/assets/images/2016-07-10/piOne.jpg)
</div>

### Iteration One
The aim of the first iteration was to enable a vocal alert to be sounded on a Sonos speaker based on events set up on [DataDog](https://www.datadoghq.com). This was done forking the code from [sonos-http-api](https://github.com/jishi/node-sonos-http-api) to make a sonos server/api, [Voice RSS](http://www.voicerss.org/) for the vocal mp3, writing our own code to write an API and the logic about what was to be said across the Sonos. 
   
We test drove our code, pairing using a red, green, refactor pattern. Once it was shown to be working, [ngrok](https://ngrok.com) was used to produce a secure url to configure a DataDog webhook to, using the webhook integration.

The code for this can be found [here](href="https://github.com/sonos-alerts) with all current instructions on how to work it. The DataDog details are currently not included.