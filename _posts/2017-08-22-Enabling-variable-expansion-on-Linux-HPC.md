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

Remember how we can auto complete the bash commands on terminal? and how double tab gives you all available options for a matching pattern? Saves a lot of time typing and searching for a command in Linux and increases your efficiency. It is also possible to do this with the variables, whether `env` (preset variables) or the custom variables that are initiated by the `.bashrc` file. To achieve this, simply add these 2 lines in your `.bashrc` file

```
shopt -s direxpand
shopt -s cdable_vars
```
