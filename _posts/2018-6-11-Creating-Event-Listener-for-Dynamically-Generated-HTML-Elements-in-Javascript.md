---
published: true
layout: post
comments: true
title: Create Event Listener for Dynamically Generated HTML Elements in Javascript
date: "2018-06-11 22:59:55 -0400"
categories: Javascript
---


For generated dynamic HTML elements, if you try to create an event listener in HTML for them, it usually won't work. The correct way is to create event listener in your Javascript file, like so:

```javascript
yourElement.addEventListener("click", yourEventFunction, false);
```

This way, a `click` event listener is created in your Javascript file and the `youEventFunction` will be executed once the `yourElement` is clicked.
