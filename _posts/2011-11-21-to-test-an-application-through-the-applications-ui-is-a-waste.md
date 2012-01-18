---
layout: post
title: To test an application through the applications UI is a waste
tags:
- Sbe
- unit test
status: publish
type: post
published: true
meta:
  _edit_last: '1'
---
I once heard that "Every time you start the debugger, the life of a unit test is lost". How very true.

Why do I still see  many colleagues for every change in the code, redeploy and restart the application. Just to verify a code change. What a waste!

Every time you test your code using the GUI, a test is lost. And a lot of time is wasted.  How much time does take to get you to the point that you can verify your code through the application? I guess 30 seconds to a few minutes is a fair estimate. Compare that with a proper unit test that run in tenth of a second. Every time.  It was 2003 that <a title="Bye debugger" href="http://weblogs.java.net/blog/sspielman/archive/2003/10/dear_johneri_me.html" target="_blank">Sue Spielman said her farewell to the debugger</a>.

I say we should start by saying goodbye to our manual GUI testing, and at the same time say hello to short test-cycles too.  If you start TDD or BDD, your time spent at the keyboard should be so much more interesting. To enter the same data in the GUI is only dull and repetitive. At worst, it is error prone. How fair is a test that is manual? Do you expect any other craftsman to do this? Would a carpenter test by putting everything together for each nail? Or would he test nail by nail and then module by module?

This leads to Iterative vs Incremental development. Let's talk about that too.
