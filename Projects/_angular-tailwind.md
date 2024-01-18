---
slug: "/projects/angular-tailwind-atomic/"
title: Applying Atomic Design with Tailblocks and Angular
description: "Developing an Open Sourced Angular library by implementing Atomic 2.0 ideas on to the Tailwind CSS framework"
author: "Steven Fewster"
category: "code"
cover: slidebean-hYN111MD_-M-unsplash.jpg
date: 1970-01-01
---

## What problem are we trying to solve?

None really.  Thsi project is more an amalgam of Atomic 2.0 ideas [as can be seen here], and Tailblocks which is some components built with TailwindCSS - a utility-first framework.
There's a lot to break down in that with some terms with which you might be unfamiliar, but suffice it to say that if you're seen how Bootstrap or Angular Material lay out their documentation - I would like to provide the same developer experience for ngTailblocks.
Also note, I haven't checked to see if this is already in existence, this project is very much: for me; for my projects; that I hope maybe others will benefit from.  I'll need to choose the appropriate license on Github/npm to underline that fact!

## Getting started
The Atomic method breaks down in to:
1. Atoms - the smallest useful indivisible unit.
2. Molecules
...
5. Organisms - A complete page, or page-like object or component.
As TailwindCSS pretty much provides Atoms, and Tailblocks provides Organisms, our job is to bridge the gap between those two with documentation and re-usable components.
As of Angular 14 we've had access to standalone components, moving away from the "module"-like boiler-plate required by earlier versions.  My original plan was to use SCAMs (self-contained Angular Modules) much as you'd see with current versions (at the time of writing) of ngBootstrap or Angular Material, but it feels like it would be a missed opportunity not to use standalone components as they're part of the official Angular 15 release.
## Part 1: All Tailblocks to Pages
This might seem counter-intuitive to the atoms first approach, but the idea is that from crafting the tailblocks as is, we can then divide them further until we're left with items that can't be broken down further without re-writing TailwindCSS classes, which we don't want to do.