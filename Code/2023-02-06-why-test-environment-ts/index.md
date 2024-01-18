---
slug: "/code/why-test-environment-ts/"
date: "2023-02-06"
title: Why would you want to write a unit test for environment.ts
description: With Angular I've been caught out more than once with build failing in prod because I've not synced environment.ts and environment.prod.ts - so write a unit test
author: "Steven Fewster"
category: "code"
cover: ./mac-and-code.jpg
---

The following is pretty basic but should at least catch those instances when you're deploying for a prod build and get caught out with missing environment variables.  It's happened to me a few times and if you pair it with something like Husky you'll catch the error BEFORE it makes the build stage.

Who knows? Maybe your build servers and performant and NOT flakey, I'm sure they exist. In which case just you can just fire off another change.  This could at least save you some time having to ask for approval multiple times.

NB: I'm aware that environment.ts will be replaced with environment.prod.ts at build time for production builds and that's fine.  It'll be comparing the same file with itself, it's more important to pick up the issue before that point.


```js
// environment.spec.ts
import { environment as Local } from './environment.ts';
import { environment as Prod } from './environment.prod.ts';

describe('Environment variables:', () => {
    it('should have the same configs in local as in prod', () => {
        expect(Object.keys(Local).toEqual(Object.keys(Prod)));
    })
});
```
