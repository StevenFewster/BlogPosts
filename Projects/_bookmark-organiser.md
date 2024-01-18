---
slug: "/projects/bookmark-organiser/"
title: Simple Browser Bookmark Organiser
description: "Written in Angular with Angular Material, allow users to upload their bookmarks.xml file and prune and organise with ease"
author: "Steven Fewster"
category: "code"
cover: slidebean-hYN111MD_-M-unsplash.jpg
date: 1970-01-01
---

## What problem are we trying to solve?
Moving jobs occasionally means that, with the best will in the world, your bookmarks might end up in a bit of a state.  Whether it's because you've got a bunch of work intranet links that you no longer have access to, or a bunch of items that you've saved to read later that have now moved or been deleted, some easy to use method of sorting them should be do-able.
## What features are we going to have?
* Keep all process offline, for user privacy
* No tracking/analytics (same as above)
* Import browsser bookmarks file (with explainer)
* Ping the URLs to verify Valid/Moved/Likely Intranet
* Some bulk organizing options, e.g. delete all dead links
* Easy drag and drop interface for creating and organising folders
* Automated suggestions???
* Export bookmarks file for re-import to the browser

``` proxy.conf.json
{
    "/v1": {
        "target": "https://...",
        "secure": false,
        "changeOrigin": true,
        "logLevel": "debug",
        "pathRewrite": {
            "^/id": "https://.../id"
        }
    }
}
```