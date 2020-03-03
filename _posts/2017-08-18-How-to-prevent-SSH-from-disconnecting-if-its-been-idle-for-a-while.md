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

If you're using HPC, chances are that your University/Sysadmin has a policy about how long you can stay inactive with the established SSH connection. If you are frustrated with this automatic disconnections, here is a way to prevent this. You can either:

```
ssh -o "ServerAliveInterval 60" -X username@server.edu
```

or create a file in ~/.ssh/config with the following line:

```
ServerAliveInterval 60
```

This will enable ssh client keepalives. The above line will send an ssh keepalive every 60 seconds that will prevent network devices from considering the session as idle.

_Source_: [https://superuser.com/a/699680/173980](https://superuser.com/a/699680/173980)
