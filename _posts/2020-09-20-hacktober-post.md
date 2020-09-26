---
layout: post
title: Hacktober Hints
description: "Links and tips for how to take part in Hacktober and where to find repositories to contribute to."
date: 2020-09-20
cover: "/assets/blog_header.jpg"
image: "assets/img/2020-09-20/twitter.jpg"
categories: [tech]
comments: false
share: true
---

----
<center>
<h3> Contributing to Open Source For Swag </h3>
</center>

---
<br/>

October has come around quickly, which means it's time to turn that GitHub graph green, find projects that need help and earn a t-shirt and stickers for your hard efforts. This post goes through what Hacktober is, how to make a contribution and a few resources for finding projects to contribute to.

## What is Hacktoberfest and how to sign up

Hacktoberfest is an event where the aim is to encourage participation on the open source community. In exchange for a number of pull requests on OSS repositories, participants are rewarded with a t-shirt and some stickers. 

To sign up, <a href="https://hacktoberfest.digitalocean.com/" target="_blank"> head over to the Hacktoberfest website</a>.

<br/>

## How to contribute to a repository

Contributions can come in many forms. You can contribute code changes, correct spelling, write documentation, raise issues, conduct testing and more. All forms of contributions are incredibly valuable and appreciated.

#### Check the contribution guidelines of the projects

Open Source repositories often have contribution guidelines. This is often documented in a `contribution.md` file, and outlines what behaviours are expected and what to do when contributing to the project.

#### Make it clear on any related issues that you are picking up the work

Check the issues tab on the project to see if the changes you want to make are highlighted in there as a bug, feature or otherwise. Check that no one else has picked up the work and that it is still available to work on. If it is, make a comment that you are picking up the work and mark it as `in progress` with a label.

#### Fork the repository

<a href="https://guides.github.com/activities/forking/" target="_blank">Fork the repository</a> and clone it locally. <a href="https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/configuring-a-remote-for-a-fork" target="_blank">Configure your remote fork to have the original projects main branch as it's upstream.</a> If you regularly pull in changes from this remote "upstream" repository, your fork will remain up to date, reducing the chance of later complex merge conflicts.

#### Create a branch

In your forked repository create a branch, which is named according to the contribution guidelines for the repository. If there are no guidelines available, give your branch a short name that summarises your changes.

#### Clear commits

While working on your changes, make sure to keep commits small and clear. If possible, each commit should be a change which builds and has any tests passing. There are a few advantages to having small, clear commits. One of which is that the owners of the repositories will be able to read through your commits when a PR is raised to see what changes you made, in what order and what your thought processes were.

#### Test your changes

Whether manually or not, test your changes and gather evidence of them working. Run any existing tests as well to ensure the project is still working.

#### Be detailed when raising the Pull Request

You can raise a Pull Request at the end of your changes, or open a draft pull request early so that others can see your changes as they progress. When filling out the details of the Pull Request, I would advise including the following:

- A reference to any issue you are addressing. This is done using a # followed by the number of your issue. For example `#97`.
- A short description of the problem you are solving and the benefits of your changes.
- Evidence of your changes working. This can include screen shots from manual tests and instructions for replicating the result locally.

#### Double check you've met the contribution guidelines

Go back to the contribution guidelines and check that you've met the instructions/requirements outlined in them. 

<br/>

## Where to find repositories to contribute to

There are a lot of places online to find places to contribute. Here are a few of the resources I've found that are available for new / first-time contributors:

#### <a href="https://github.com/firstcontributions/first-contributions" target="_blank">First Contributions</a>

First contributions is a repository made for those who have never contributed to OSS before. Fork, create a branch, add your name to the `Contributors.md` and raise a pull request.

#### <a href="https://github.com/MunGell/awesome-for-beginners" target="_blank">Awesome First PR Opportunities</a>

This repository lists projects by language that have labels indicating that there are issues suitable for those new to contributing to open source. It also lists the labels to search for within the issues of each project.

#### <a href="https://up-for-grabs.net/#/" target="_blank">Up For Grabs</a>

A site where you can search for issues that available by label, langauge, tag or name. It shows projects which have issues that indicate they are looking for contributors. This is for all levels and not only beginner friendly issues.

#### <a href="https://www.firsttimersonly.com/" target="_blank">First Timers Only</a>

This page have a number of resources for first time contributors.

#### GitHub labels.

There are a number of labels which are attached to issues, indicating they are looking for help and what level the problems may be available for. Some include:

- `beginner`
- `beginner-friendly`
- `first-timers-only`
- `first-contribution`
- `good-first-issue`
- `help-wanted`
- `up-for-grabs`

<br/>

## Staying safe in open source

In general, people want to help you and encourage you to learn in a safe space. None the less, not all online spaces are safe and welcoming. For the most part, if it is indicated that a project has issues suited for beginners and first time contributors, then it's a project you will be treated well in.

I personally would advise to **check that the project has a code of conduct before contributing**. Hopefully this code of conduct will outline what you can do if you experience any behaviour that makes you feel uncomfortable or that is unsupportive. In this case, if the worst happens you know that you will be supportive and what support you can expect to recieve.

<br/>

## Extra Resources
- <a href="http://opensource.guide/how-to-contribute/" target="_blank">How to Contribute to Open Source</a>
- <a href="https://chris.beams.io/posts/git-commit/" target="_blank">How to Write a Git Commit Message</a>

## When October Ends

Hacktober is an awesome initiative and can be great fun to take part in. Open Source isn't just for Hacktoberfest. These labels and resources are available all year, and though you won't get a t-shirt or stickers the rest of the year for your efforts, contributing is rewarding in it's own right.

I hope that the experiences you have in October encourage you to keep contributing and taking part all year around.

_Happy Hacking_

_Jess_

---


<div style="text-align:center; width:20%; margin-left: 10%;" markdown="1">
<img src="{{site.baseurl}}/assets/img/logo.png" alt="Logo">
</div>
