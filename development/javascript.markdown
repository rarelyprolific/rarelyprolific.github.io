---
title: JavaScript Development
layout: post
---

One of the technical goals I've set for myself in 2017 is to get to know JavaScript better. I'm reasonably happy with vanilla JavaScript,
using jQuery and the basics of KnockoutJS but the world of JavaScript moves fast. There are a wealth of new JavaScript frameworks,
tools and development environments as well as a busy roadmap of new features set to hit the core language in the near future.

**So I'm not attempting to learn or even be aware of everything.** Basically there is too much going on. There are not enough
hours in the day and I also want to reserve some learning time for non-JavaScript technologies.

What I am going to concentrate on is looking for tools, frameworks and libraries which assist and drive you towards developing high
quality JavaScript. It's really easy to write really bad JavaScript.. I'd like
to [fall in the pit of success](https://blog.codinghorror.com/falling-into-the-pit-of-success/) more often.

I'm also going to favour concepts which are either part of the core language or are likely to be included in it in the future. My theory
is that frameworks come and go *(fairly rapidly in some cases)* and they often share features *(such as two-way databinding between JavaScript
models and the UI)* even if they architect them differently. I'm also interested in finding out if we ever use JavaScript too much and if
there are sometimes better solutions.

**First question..**

## Which editor should I use to write JavaScript?

There are many choices out there but I'll start with a couple I've ruled out and why:

- **Visual Studio** - VS 2015 is my weapon of choice for most work. It generally does everything well and is the swiss-army knife of software
development. So why not here? Firstly, it likes you to structure your code via projects and solutions which I don't think is optimal for
JavaScript work, which usually just sits inside a folder hierarchy in the file system *(Although I know, technically, you can do this with VS by
pointing it at a "web site")*. Secondly, it is fairly heavy on your system resources. I need something fast,
light and responsive so I can achieve the most [rapid feedback](https://mlafeldt.github.io/blog/fast-feedback-is-everything/) on any code I'm working on.

- **Notepad** *or any basic text editor* - Writing JavaScript can be **very** error prone. It's a dynamic language so inadvertent typos often result
in undesired behaviour rather than explicit runtime errors. Therefore to save frustration in the future I want an editor which understands
JavaScript, can highlight my errors and also make good suggestions.

I've picked three open-source editors to look into more closely. These are:

- **Brackets** by Adobe
- **Atom** by GitHub
- **Visual Studio Code** by Microsoft
