---
title: "Lifecycle and Event-Based Testing for Android Applications"
categories: research
tags: android
excerpt: "A comprehensive framework to automating testing of events in Android applications." 
header:
  teaser: simone-teaser.png
published: true
--- 

{% include base_path %}


![slide]({{ base_path }}/images/simone-teaser.png)
{: .align-center}

Great work on "Lifecycle and Event-Based Testing for Android Applications" by
Simone Graziussi, the student I've co-advised with Luciano Baresi.

Simone has written an [excellent thesis](https://github.com/Simone3/Thesis) that
focussed on  two particular challenges of mobile testing that have been largely
overlooked to date, lifecycle management and event concurrency.

First of its kind, the approach presents static code analysis to recognize
possible misuses of app components, and a dynamic technique that allows the
developer to drive the application lifecycle to test its robustness.

His thesis develops an event-based testing approach that allows to observe
several events during the application execution and to express consistency
checks on their stream by means of a proposed temporal assertions language.

Together, the thesis forms a __comprehensive framework__ to automating testing of
events in Android applications, allowing to express existence, ordering,
causality and quantification conditions on them, as well as to better control
the critical lifecycle transitions.

__P.S.:__ A concise view of the work is available in the [poster]({{ base_path
}}/images/2016-poster.pdf) presented at the Open House 2016 [^1] @ DEIB of the
Politecnico di Milano.

[^1]: The Open House event disseminates and promotes research to students and companies by presenting scientific activities, teaching courses and job opportunities that a Master of Science Degree in Computer Science and Engineering offers. 

