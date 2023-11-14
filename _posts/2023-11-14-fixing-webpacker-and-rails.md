---
layout: post
title: Fixing Webpacker and Rails
categories: []
tags: []
status: publish
type: post
published: true
meta: {}
---
Recently was working with maintenace on some older Rails 6 apps. Both had issues deploying with this error:

```
Error: error:0308010c:digital envelope routines::unsupported
```

The issue is related to the version of Node. Switching to 16.16.0 fixed the issue. For Heroku adjust your package.json:

```
"engines": {
  "node": "16.16.0"
}
```
