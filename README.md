# Jessica White's Blog Page

![JessWhite Deploy](https://github.com/wordshaker/jesswhite_4/workflows/JessWhite%20Deploy/badge.svg?branch=main)

This is for the blog page [jesswhite.co.uk](https://jesswhite.co.uk).

# Contents
 - [Local Development](#local-development)
   - [Setup Jekyll](#setup-jekyll)
   - [Building Locally](#building-locally)
   - [Running Locally](#running-locally)
   - [Gotchas](#gotchas)
 - [Build Tool](#build-tool)

<br/>

# Local Development 

## Setup Jekyll

- [Follow the instruction to set up Jekyll on your machine](https://jekyllrb.com/docs/)

## Building Locally

- Run `bundle exec jekyll build` to build the project

## Running Locally

To run the project locally use the command `bundle exec jekyll serve` in the terminal of your choice. This make the site available on `http://localhost:4000/`. Access that address in the browser of your choice to see your local version of the website.

## Gotchas

- When running locally, you will only see posts that are in the past or dated for the current day.

<br/>

# Build Tool

GitHub Actions is set up to build and run tests from Pull Requests so that I can ensure the project builds and tests pass from any changes made within branches before they are merged in. 

GitHub Actions is also used to deploy on merge into main.

![JessWhite Deploy](https://github.com/wordshaker/jesswhite_4/workflows/JessWhite%20Deploy/badge.svg?branch=main)
