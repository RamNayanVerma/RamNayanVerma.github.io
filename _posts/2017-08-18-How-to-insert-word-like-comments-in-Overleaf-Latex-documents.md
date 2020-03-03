---
layout: post
title: This is my first blog!
excerpt: "stating blog post, what should I write about?"
date: 2013-03-01T15:21:00+00:00
modified: 2013-03-01T15:21:00+00:00
tags: [Arun Seetharam, hack, bioinformatics, bash]
categories: [bioinformatics]
comments: true
#image:
#  feature: image.jpg
#  credit: Arun Seetharam
#  creditlink: http://aseetharam.github.io
---

There is a `todo` package that can be used for this purpose. Simply add these lines to your document and you can leave comments with \todo commands.

\usepackage{geometry}


The above package will be used in most documents, so no need to add it if its already there

\usepackage[colorinlistoftodos]{todonotes}


by default it will be on right, to put it on left (if you don't have room beacuse of margins) use

\reversemarginpar


For commenting

\todo{this is an example comment}


Comments will be show as follows:
