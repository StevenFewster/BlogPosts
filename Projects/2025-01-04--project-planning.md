---
slug: "/projects/cranky-hippo/"
title: Project Cranky Hippo
description: "Planning stage for a new project to help promote live events/scanning fliers"
author: "Steven Fewster"
category: "projects"
date: 2025-01-04
cover: ./zhao-yangjun-sRCDREoEqAA-unsplash.jpg
attr:
  sourceName: Zhao Yangjun
  sourceLink: https://unsplash.com/@youngjun420?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash
  siteName: Unsplash
  siteLink: https://unsplash.com/photos/a-toy-hippopotamus-with-its-mouth-open-sRCDREoEqAA?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash
---

## What's In A Name

I've been caught in a name trap too many times, so let's just go with _Adjective Noun_ type of naming convention so that we can easily pivot later and don't to our usual of buying a domain name that we then let lapse. Ladies and Gents, I give you: _Project Cranky Hippo_.

## Planning

It's sensible to have at least some sort of structure to how to attack a project that's going to be a reasonable size and go on for a decent length of time. In software it's very common to have things such as "Definition of Done" and "Acceptance Criteria" and they serve a useful purpose. However, we don't want to tie ourselves down with undue administrative overhead.

In steps GitHub. We're going to be using it as a code repository, and it comes bundled with some issue tracking type stuff, so it seems a no-brainer to keep it stored in one place. Again, we need to start a a high level, then break them down into smaller bite-sized challenges.

Having a reasonable idea of what I want to use with regards development stack, that will also inform the approach.

## Milestones

These should be driven by our WHY [discussed earlier](http://localhost:4321/editorials/starting-with-why/) and bigger, bolder complete things. For this project it breaks down as follows:

- Web application which allows registration and log in
- Screen to add event date/time
- Listing upcoming events on homepage
- Make events searchable by location/proximity
- Adding existing rss/xml feeds to applications
- Provide mobile version of web app
- New screen to capture and add fliers/posters

## Breaking down that first Milestone

We need some ACs and a definition of done for the first Milestone, which will likely lead to more detailed requirements.

> Web application which allows registration and log in

We're going to be using [WASP Framework](https://wasp-lang.dev/), so this is going to be relatively straight-forward.

Done as far as we're concerned for this Milestone is:

- Application is deployed to a publicly accessible server
- Pipeline automatically deploys on push
- Simply styled application view
- User is able to create an account and log in
- Whitelisted usernames/email addresses

## Tasks (T) and Features (F)

- (T) Crete Git project to host code and management
- (T) Create project and commit to git
- (F) Update code to only allow registrations from xxx.com
- (F) Add basic styling to application
- (T) Create pipeline and deployment target
- (AC) verify ACs are met

Now those are done, we need to get started with the first task and then add in the rest of our milestones and features so that we can mark them done as we go. I feel this is lightweight, but robust enough for us feel progress being made.

Steven.
