---
layout: post
title: Maintaining Repositories - A Hacktober Story
description: "A log of things I've learnt about and will consider for future repository maintainence based on my experience of being a maintainer of repositories taking part in Hacktoberfest. This post will be updated throughout October 2020."
date: 2020-10-04
cover: "/assets/blog_header.jpg"
image: "assets/img/2020-10-04/twitter.jpg"
categories: [tech]
comments: false
share: true
---

----
<center>
<h3> Lessons learned from being a maintainer. </h3>
</center>

---
<br/>

This year I have been hands on with maintaining the .NET Notts and DDD East Midlands repositories over the Hacktober period. There are a number of considerations when managing these repositories that I am documenting in this post.

<center>
<h2>THIS POST IS BEING UPDATED THROUGHOUT OCTOBER. </h2>
</center>


<h2>Quick Links:</h2>

- [What I've learnt as a maintainer](#what-ive-learnt-as-a-maintainer)
  - [Use the right licence](#use-the-right-licence)
  - [Have a Code Of Conduct in place](#have-a-code-of-conduct-in-place)
  - [Guide for how to run the code and locally](#guide-for-how-to-run-the-code-and-locally)
  - [Contribution Guidelines](#contribution-guidelines)
    - [Avoiding PR clashes](#avoiding-pr-clashes)
    - [Maintaining consistency](#maintaining-consistency)
  - [GitHub Templates](#github-templates)
  - [Branch Protection](#branch-protection)
  - [Setting up CI and CD](#setting-up-ci-and-cd)
  - [The many types of contribution](#the-many-types-of-contribution)
  - [Tone of voice](#tone-of-voice)


<br/>

## What I've learnt as a maintainer

The next sections explore at a high level, what I have learnt about as a maintainer. I wanted to share these as it may be useful to any of you that are thinking of looking after open source repositories.

<br/>

### Use the right licence

Licencing is a tricky topic, but as a maintainer you need to ensure a licence is in place for the code you are caring for. There are many resources on this topic including the documentation <a href="https://opensource.org/licenses" target="_blank">on the OpenSource.Org Website.</a>

I'd highly recommend watching <a href="https://www.youtube.com/watch?v=OV94p_kB-Lg" target="_blank">this talk by Jeff Strauss titled - What You Need to Know About Open Source—Trust Me, I’m a Lawyer</a>. I've watched this talk 3 times in person, back when we could watch talks in person. Jeff clearly talks through the different types of licence, what they mean and how they impact you as a code owner.

Not only does this enforce how your software can be used, but also many contributors will avoid contributing to repositories that don't have a licence.

<br/>

### Have a Code Of Conduct in place

The Code of Conduct is for maintainers as well as contributors. Having a code of conduct makes it clear what behaviour and language is expected of all those taking part in the repository. It also states what will happen if anyone behaves in a way that is not allowable by the maintainers.

This means all those contributing are prewarned to the consequences of actions that make others feel targeted, uncomfortable or abused. If anyone is made to feel unsafe, there are instructions for how to report the behaviour that has made them feel that way.

All in all this document helps provide the information necessary to try to preserve a good culture in the repositories you are maintaining and make sure that everyone taking part has a good experience.

<br/>

### Guide for how to run the code and locally

Having a clear guide on how to run the code locally will help anyone who wants to contribute to your repository test their work before pushing up changes. By helping your contributors run the code and tests on their locally machines, you help them to ensure they are pushing up code that meets the requirements without breaking anything else unexpectedly.

I have chosen to put these guides in the README of the repository. The repository is a guaranteed place that all contributors will visit and having a guide here, also keeps the guide next to the code it affects.

<br/>

### Contribution Guidelines

These guidelines inform contributors what they need to do to make changes to the repository. 

#### Avoiding PR clashes

In the .NET Notts repositories we ask that people request to make changes on an existing issue or an issue they have raised. Once a maintainer has assigned the change to them, then they can raise a pull request.

The reason for this is we had a number of pull requests being raised for the same issue from numerous people. We needed a fair way to decide who's changes went through, and to be transparent about what this process was.

#### Maintaining consistency

By documenting how you want individuals to contribute to your repository, it increases the changes that there will be consistency between the different contributions the repository received. This can include things like branch name structure, whether you want contributors to fork the repo opposed to branching straight from the main repo or if you want any evidence of changes.

<br/>

### GitHub Templates

Adding <a href="https://docs.github.com/en/free-pro-team@latest/github/building-a-strong-community/about-issue-and-pull-request-templates" target="_blank">issue and pull request templates</a> to your repository helps ensure that all Pull Requests and Issues are consistent and contain the information you need. You can outline headings and put down some description of what you would like those contributing to put under each heading.

<br/>

### Branch Protection

In the Settings of the GitHub repository as a maintainer you can protect your branches under a number of criteria. You can set it up so that pull requests can't be merged without build checks passing, reviews from certain people or a set number of reviews.

These rules ensure that unwanted changes can't be merged into your main branch.

<br/>

### Setting up CI and CD

For pull requests, you can set up builds and test runs to check that the builds and tests haven't failed on any changes made. Repositories can also be set up to deploy when changes are merged into the main branch. This stops any unnecessary manual effort.

<br/>

### The many types of contribution

There are lots of different types of contribution that can be made to a repository including:

- Bug fixes
- Feature contributions
- Designs 
- Adding tests 
- Accessibility testing and checks
- UI and UX assessments

In the contribution guidelines it is good to be clear how these changes can be made.

<br/>

### Tone of voice

When taking care of a repository you need to determine your tone of voice when talking to contributors. Make sure its constructive, and not unkind. 

Your tone of voice determines the culture of the repository as a whole. The maintainers are the example for what communications and behaviours should look like.

<br/>


_Stay Safe,_

_Jess_


---

<div style="text-align:center; width:20%; margin-left: 10%;" markdown="1">
<img src="{{site.baseurl}}/assets/img/logo.png" alt="Logo">
</div>
