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

If you want to quickly count the number of reads in a fastq file, you can count the total number of line and divide them by 4. However, when you want to generate a nice table for the reads when writing a report, this will be a inconvenience. So, here is my simple bash script that does this job

```bash
#!/bin/bash
if [ $# -lt 1 ] ; then
	echo ""
	echo "usage: count_fastq.sh [fastq_file1] <fastq_file2> ..|| *.fastq"
	echo "counts the number of reads in a fastq file"
	echo ""
	exit 0
fi

filear=${@};
for i in ${filear[@]}
do
lines=$(wc -l $i|cut -d " " -f 1)
count=$(($lines / 4))
echo -n -e "\t$i : "
echo "$count"  | \
sed -r '
  :L
  s=([0-9]+)([0-9]{3})=\1,\2=
  t L'
done
```
