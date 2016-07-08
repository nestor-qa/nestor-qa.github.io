---
layout: page
title: Backbone Events
---

The web interface uses several _BackBone.JS javascript events_, documented here for
simplicity.

## List of events

### Event: nestor:navigationtree:project_changed

### Event: nestor:navigationtree_changed

### Event: project:position

#### When it is triggered

Triggered when a new project is positioned in the header. The ProjectsCollection sends
an HTTP request to the back end. Once it is done and successful, the collection triggers
this event.

#### Who is affected

In router.js, there is a global hook. Whenever the event is triggered, and if the
current view is not the view projects view, then the user is redirected to the
specification page.


