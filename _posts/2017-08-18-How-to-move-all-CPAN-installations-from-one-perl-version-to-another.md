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

cpan as a built-in option for this purpose. First, create a bundle of all existing packages. For this, load the older perl version which will be the source for all cpan modules:

```
module load perl/5.22.1
perl -MCPAN -eautobundle
```

This will print all the CPAN modules that it puts in the bundle. Once complete, you'll see:

```
Wrote bundle file
    /path/to/current/dir/Snapshot_2017_05_09_00.pm
```

Now, unload the older perl and load newer perl:

```
module purge
module load perl/5.24.0
```

And install modules:

```
perl -MCPAN -e 'install Bundle::Snapshot_2017_05_09_00'
```

It should install all CPAN modules in the bundle!
