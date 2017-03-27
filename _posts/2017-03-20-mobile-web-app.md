---
title: "Why passing data inside a mobile app is difficult?"
categories: tech
tags: android
excerpt: "The 'web app' metaphor helps to grasp Android app structure. Makes clear why passing data between activities is difficult." 
header:
  teaser: app_structure_overview.png
comments: true
published: true
---

{% include base_path %}

> "The solutions all are simple... After you've already arrived at them. But they're simple only when you already know what they are."
<cite>Robert M. Pirsig, "Zen and the Art of Motorcycle Maintenance"</cite> 
{: .small .text-left}


![Kovacs shot put]({{ base_path }}/images/kovacs_2016.jpg){: .align-center}


You're learning to develop Android apps and very early on you're stuck. You've faced
a problem that __you just can't easily pass data within your app__. That's
unexpected. And solutions seem to be much more complex than you've hoped for in
this beginner stage. It feels like you're just wasting time trying to read all
the docs. What's going on?

I suspect that some fundamental concept about app structure has not been
explained to you. Let me try to set it straight.

First, let's see where you find yourself. You've [built your first
app](https://developer.android.com/training/basics/firstapp/index.html)
following the Google developer tutorial. Added a few simple activity classes
that represent individual screens of your app.  And now you wish to send some
data between them (beyond a string of text). Say, a captured picture, an object of
a class `Person` filled with some contact details, or an `ArrayList` of
records. You try to put it in an `Intent`, but it's not working.  (By the way,
you're still confused whether intents are to open other activities or to send
data between them). 

You promptly discover that intents can only carry little additional
information, mostly primitive types, to be packed as key-value pairs.  You go
to _Stack Overflow_ to discover that you've got to use [something
`Parcelable`](http://stackoverflow.com/a/2141166/3419014) to send objects
between
activities.  

-- "What is that? I've just started learning? Can't we have it simpler?"

You go back to Google tutorials that give you options to save app data in
[Key-Value Sets, files, or SQL
Databases](https://developer.android.com/training/basics/data-storage/index.html).

-- "Isn't that an overkill for just sharing simple pieces of data within a
trivial app?  Come on!"

## The "web app" metaphor

Here you need to pause and understand that you probably miss something essential
about Android apps and their structure. The most useful metaphor
that I have to share with you is this:

think of __your phone as a web browser__ and __your app as a web app -- a
collection of web pages__.[^1] 

In a web app each page is standalone, the data it needs is loaded from a server
or other resources on the web (it does not come directly from the preceding
page).  Each page knows to open another one using links. As you follow to open
the next page, it takes place of the previous one that gets closed.

Mobile apps essentially follow the same structure. __Each activity is
standalone, responsible for obtaining its own resources, just like a web
page.__ Starting from the launcher activity (app's home page), user navigates
around the app using "links" to reach other activities. If a phone call arrives,
the app is not closed, the "browsing history" with the latest activity on top
is preserved in the background by the operating system (imagine a web page
covered with a new opened tab). After the calling app is closed, you see your
app as you left it.  
The only difference is that our app can only be shown in "one tab" of our
"browser", and only one page (activity) of our app is visible at a time. 

What you might have imagined about Android app structure being a monolith
application made of different Java classes, is actually several smaller
independent "apps" (activities) packed together.

## How is it useful?

Now you should start to see why sending data between activities is not trivial.
It's about connecting smaller independent "apps". And trying to put more data
in an `Intent` is like trying to send pictures between two web pages, instead of
uploading a picture to the server and make it accessible to both.  You also
start to see why do you might need `Services` for long-running operations.

Armed with a good metaphor you don't waste your time hacking workarounds and
getting red eyes after browsing dozens of _Stack Overflow_ questions/answers, and
instead focus on learning the stuff you'll need time and again (such as, for
example, working with SQL Databases).

![Kovacs happy]({{ base_path }}/images/kovacs_2016_2.jpg){: .align-center}

__P.S.:__ Can you do me a favor and leave a comment about any other useful
Android metaphor you've come across?


[^1]: I am not talking about web-based mobile apps right now, just in general.


