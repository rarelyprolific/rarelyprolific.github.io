---
layout: post
title:  "Innovation, learning and biting off more than you can chew"
date:   2017-01-25 21:55:00 +0000
permalink: "innovation-and-learning"
---

There is a constant drive for innovation in software development. Organisations want to be seen to be embracing new technology and
most developers have a built-in desire to play with new toys.

Here's a scenario I was involved in a few years ago.

We had a trusty ASP.NET WebForms application which performed a few simple but vital internal business functions. It didn't look very nice
but it was used by a few users who seemed to be content with it and we had no complaints *(and we definately got complaints about the
stuff they didn't like!)*. The back-end code was a little gnarly but generally it worked well and did it's job.

Then we had to change a few services and databases which propagated data around our systems. This meant we also had to modify our
WebForms application to maintain compatibility. After some analysis it became apparent that we would have to make some fairly
extensive changes to the nasty back-end code of the application as the shape of the source data was now significantly different.

So we already had a reasonably large task ahead of us. But there was also a nagging feeling that this was a really ugly old legacy application.
We could do all the necessary work rewriting the backend code but it would still look like a 1990's web application on the front end.
None of the users would notice anything had changed, which could be viewed as a positive, but there would be no recognition of the amount
of blood and sweat it had taken to upgrade the application.

We decided it would be really good if we could give the front-end of the application an upgrade too. We were already mashing up the code so
why not! Everyone was using JavaScript these days so we should really be doing some of that too. We also want a modern looking design and
smooth data refreshes via AJAX instead of reloading entire pages.

This is all good stuff but our reasonably large task had now grown to significantly massive. Even though we didn't realise this at the time.
To be fair, we did realise that changing both the back-end data processing and front-end design would be a fairly large job but if we just
did the back-end first we wouldn't get the chance to do the front-end design we really wanted to work on.

As it happened we succeeded with what we set out to do and we got it all done by the required deadline. The back-end code was upgraded so it
did exactly what it needed to do (it would have been game over if this wasn't the case to be honest).

The front-end was.. interesting! We had indeed given the application a whole new user interface. It was a little rough around the edges but definately looked more modern.
It worked but we had a few niggly user experience issues such as the page loading a half blank page instantly and then the data appearing a couple of
seconds later when an AJAX request returned.

All things considered, was this a successful project though? If you look only at the end result I think we won. It worked. It wasn't perfect but the
original application didn't have great UX either, we just had slightly different issues in the new version.

But I'm a big believer in the concept of EVERYTHING having a cost. Especially in software development. In fact, modern software methodologies often tell
us to ["do the simplest thing that could possibly work"](http://ronjeffries.com/xprog/articles/practices/pracsimplest/). It's fair to say we completely
broke this rule and then some.

The hidden cost for us, which isn't apparent from the above explanation, is the amount of stress and pulling our hair out we had to go through to
get the front-end code working. We probably should have initially just worked on the back-end code if we were taking
an MVP ([Minimum viable product](https://en.wikipedia.org/wiki/Minimum_viable_product)) approach.

But, with hindsight, the overarching issues which exasperated the development process more than anything was:
* No one on the team knew much about JavaScript development before we started the work.
* We underestimated how much learning we would have to do "on the fly".
* We couldn't begin to anticipate some of the issues we ended up having to deal with whilst writing and debugging the code.

It's easy to judge this as an observer and ask why a bunch of developers would dive head first into problems they don't have a clue how to solve (or how
to even estimate with any degree of accuracy for that matter) but I've personally witnessed this scenario happen at more than one organisation and
with both novice and experienced developers.

I think it happens when you have a workplace culture which doesn't allocate any real time to enable developers to learn new skills.
It can happen when a developer's time is ALWAYS tied to delivering a feature, so there is no time in reserve for personal development. They can get around
this limitation by actually producing the new feature using exciting new stuff whilst learning it simultaneously. Two birds, one stone! Developers are great problem solvers after all.

But the cost is usually significantly more time spent in the debugger trying to diagnose problems based on code you don't really understand at this
point (googling stack overflow to the rescue!) in addition to the bugs you have to fix in the business logic which was always part of the task anyway. Oh, and get it done
by the same deadtime too. Stress! Argghh!

Personally I don't think this practice works. You are taking on risk which you can avoid. You may deliver on time or you may not deliver at all if you
can't get the shiny new technology to do what you need it to. Either way, you are probably going to end up putting yourself under more pressure and stress than
you need to and you aren't going to be at your best if you are doing that on a regular basis.

Part of the solution is that your organisation (if they don't already) should really have a company strategy for developer personal development. Good developers
generally learn in their own time but this behaviour should be engrained into the workplace too.

Ultimately though, developers should have the discipline to learn and try out new skills in safe environments and keep unproven technologies away from the production codebase. (I'll elaborate on techniques for doing this in a future post.)