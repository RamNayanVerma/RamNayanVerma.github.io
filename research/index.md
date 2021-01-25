---
layout: page
title: Current Projects
date: 2017-02-26T00:15:47+01:00
modified: 2017-09-02T12:30:00+01:00
excerpt: "Urminder Singh's current projects"
tags: [Urminder Singh, research, bioinformatics, evolution, machine learning]
---


<section id="table-of-contents" class="toc">
  <header>
    <h3>Overview</h3>
  </header>
<div id="drawer" markdown="1">
*  Auto generated table of contents
{:toc}
</div>
</section><!-- /#table-of-contents -->


### Role of genetic ancestry in COVID-19 susceptibility and severity

As of January 2021, the COVID-19 pandemic has infected over 98 million people and killed over [2 million worldwide](https://coronavirus.jhu.edu/map.html).
People of African and Latin ancestries in the U.S. are disproportionately [affected](https://blog.23andme.com/23andme-research/impact-disparities-of-covid-19/) by COVID-19 with respect to prevalence, morbidity, and mortality.

An individual's health is a result of complex interactions among one's [genetic](https://www.sciencemag.org/news/2020/10/found-genes-sway-course-coronavirus), environmental, and [socio-economic](https://blogs.scientificamerican.com/voices/racism-not-genetics-explains-why-black-americans-are-dying-of-covid-19/) factors.
We leveraged RNA-Seq expression data and probed differences in gene-expression among people from European and African Ancestries. Although we could not control environmental and socio-economic factors (because of lack of metadata), we found differential expression of genes implicated in COVID-19 infection.
Further, African American gene expression signatures reveal an increased number or activity of esophageal glandular cells and lung ACE2-positive basal keratinocytes.
Please read our preprint [here](https://assets.researchsquare.com/files/rs-88890/v1_stamped.pdf).

Our ongoing research, in collaboration with the COVID-19 International Research Team ([COV-IRT](https://www.cov-irt.org/)), aims to detect genetic factors that can explain the disparity of COVID-19 infection and mortality rate among different populations. 
We are particularly interested in identifying and examining the roles of human specific [orphan genes](https://elifesciences.org/articles/55136) and non-coding RNAs in COVID-19 infection.

**This research is funded by National Science Foundation grant IOS 1546858, Orphan Genes: An Untapped Genetic Reservoir of Novel Traits, and by the Center for Metabolic Biology, Iowa State University**

### Identifying novel orphan genes in human using massive RNA-Seq data

![](/images/geneslifecycle.jpg)
*Figure showing life cycle of orphan genes. Ref: [Singh, U., & Wurtele, E. S. (2020). Genetic novelty: How new genes are born. Elife, 9, e55136.](https://elifesciences.org/articles/55136)*

During evolution, genes undergo duplication and divergence and give rise to new genes.
These new genes can potentially code for [new proteins](https://en.wikipedia.org/wiki/Gene_duplication) and provide the organism with useful biological functions.
Genes resulting through the process of duplication could be traced back to their ancestral genes via [sequence homology](https://en.wikipedia.org/wiki/Sequence_homology).
However,  in every organism, a number of genes can not be traced back to any ancestral gene.  
These species-specific genes are termed [orphan genes](https://en.wikipedia.org/wiki/Orphan_gene). 
Many such orphan genes are involved in [biologically important functions](https://pubmed.ncbi.nlm.nih.gov/25151064/).
Orphan genes can arise [*de novo*](https://en.wikipedia.org/wiki/De_novo_gene_birth) from non-genic regions in the genome. 

The focus of my research is to identify and characterize novel expressed genes in humans. To achieve this goal, I am integrating and analyzing terabytes high quality of RNA-Seq datasets from massive projects like [GTEx](https://gtexportal.org/home/), [TCGA](https://portal.gdc.cancer.gov) and [SRA](https://www.ncbi.nlm.nih.gov/sra).

**This research is funded by National Science Foundation grant IOS 1546858, Orphan Genes: An Untapped Genetic Reservoir of Novel Traits, and by the Center for Metabolic Biology, Iowa State University**



### Examining cell-type specific expression of novel genes

With the advent of [single-cell sequencing](https://en.wikipedia.org/wiki/Single_cell_sequencing) it is now easy to examine transcriptome profiles at the single-cell level.
I am leading a small team to examine publicly available single-cell RNA-Seq datasets to look for cell-specific expression of novel genes.

**This research is funded by National Science Foundation grant IOS 1546858, Orphan Genes: An Untapped Genetic Reservoir of Novel Traits, and by the Center for Metabolic Biology, Iowa State University**


### A deep-generative model to integrate massive bulk expression datasets

Petabytes of RNA-Seq are available publicly via resources like NCBI-SRA.
[Integrative analysis](https://doi.org/10.1093/nar/gkz1209) of such data provides an opportunity to mine biologically essential insights.
A significant challenge of integrating RNA-Seq datasets from multiple sources is unwanted technical and biological effects.
Technical effects, such as batch-effects due to technical factors, may be controlled if the batch co-variates are known.
A significant problem arises when sources of such effects are unknown or hidden.
Methods like [SVA](https://academic.oup.com/nar/article/42/21/e161/2903156) can remove some of the unwanted variations.
New methods like [SAUCIE](https://www.krishnaswamylab.org/projects/saucie) use auto-encoders for batch correction and de-noising single-cell expression data, in an unsupervised manner.
Other deep-learning-based methods have also been developed for single-cell datasets.

I am interested in developing deep generative models for non-linear factor analysis of massive bulk RNA-Seq expression data.
In this ongoing project, I am using variational auto-encoders to model RNA-Seq count data directly and project them into smaller latent dimensions to remove unwanted variation.

**This research is funded by National Science Foundation grant IOS 1546858, Orphan Genes: An Untapped Genetic Reservoir of Novel Traits, and by the Center for Metabolic Biology, Iowa State University**



### MetaOmGraph: A tool for exploration of big omics data

![](https://raw.githubusercontent.com/urmi-21/MetaOmGraph/master/images/MOG_flowchart.png)
*Figure showing overview of MetaOmGraph tool. Ref: [Singh, U., Hur, M., Dorman, K., & Wurtele, E. S. (2020). MetaOmGraph: a workbench for interactive exploratory data analysis of large expression datasets. Nucleic acids research, 48(4), e23-e23.](https://doi.org/10.1093/nar/gkz1209)*

I am the lead developer of [MetaOmGraph](https://doi.org/10.1093/nar/gkz1209), a fully interactive exploratory data analysis software for big omics datasets.
MetaOmGraph allows user to visualize and analyze their data using a number methods in a fully interactive manner.
As data becomes complex, it is important to [explore data](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-020-02133-w) from different perspectives.
MetaOmGraph lets the user do that in an efficient and straightforward manner.
Domain experts, such as biologist, cell biologists, virologists, and medical professionals can easily analyze the data without writing any code.
MetaOmGraph is an open source project. Please see it on github [here](https://github.com/urmi-21/MetaOmGraph).

**This research is funded by National Science Foundation grant IOS 1546858, Orphan Genes: An Untapped Genetic Reservoir of Novel Traits, and by the Center for Metabolic Biology, Iowa State University**


### pyrpipe: Bioinformatics pipelines in pure-python

![](/images/pyrpipe_2.png)
*Figure showing overview of pyrpipe. Ref:[Singh, U., Li, J., Seetharam, A., & Wurtele, E. S. (2020). pyrpipe: a python package for RNA-Seq workflows. bioRxiv.](https://www.biorxiv.org/content/10.1101/2020.03.04.925818v4)*

Writing complex bioinformatics pipelines in a fully reproducible, easy-to-debug, maintainable manner can be challenging.
Often plain scripting is used to implement the pipelines, which can have many drawbacks.
I developed *pyrpipe* to provide a framework to implement RNA-Seq and other bioinformatics pipelines in pure python in an object-oriented manner.
pyrpipe provides special API classes that allow *importing* any Unix executable command in python.
All commands executed via *pyrpipe* is in this manner is automatically logged, monitored, or can be flexibly controlled using *pyrpipe* options. 
*pyrpipe* comes with API to access popular RNA-Seq tools directly from python. Using this framework, RNA-Seq processing pipelines can be intuitively coded.
*pyrpipe* pipelines could be easily extended to add new tools. Parameters can be easily managed in YAML files, which are automatically parsed by *pyrpipe*.
*pyrpipe_diagnostic* can generate in-depth reports and logs for debugging and reproducibility.
*pyrpipe* can be easily installed via conda or PyPI.
*pyrpipe* source code is available on [github](https://github.com/urmi-21/pyrpipe). 
Please read the pre-print [here](https://www.biorxiv.org/content/10.1101/2020.03.04.925818v4).

**This research is funded by National Science Foundation grant IOS 1546858, Orphan Genes: An Untapped Genetic Reservoir of Novel Traits, and by the Center for Metabolic Biology, Iowa State University**

### orfipy: Fast and flexible ORF caller

![](/images/orfipyfig.png)
*Figure showing features of orfipy. Ref: [Singh, U., & Wurtele, E. S. (2020). orfipy: a fast and flexible tool for extracting ORFs. bioRxiv.](https://www.biorxiv.org/content/10.1101/2020.10.20.348052v1)*

Identification of Open Reading Frames (ORF) is an integral step for any gene annotation pipeline.
Presently, there exist many tools for ORF identification, such as the popular [Getorf](http://emboss.sourceforge.net/apps/cvs/emboss/apps/getorf.html) and [OrfM](https://github.com/wwood/OrfM).
These tools work great but are not flexible in terms of fine-tuning ORF search.
I developed *orfipy* to solve this challenge. *orfipy* is fast and flexible.
*orfipy* reduced the total runtime of my [orphan gene prediction pipeline](https://www.biorxiv.org/content/10.1101/2019.12.17.880294v2) significantly while accurately identifying the ORFs.
*orfipy* can be easily installed via conda or PyPI.
*orfipy* source code is available on [github](https://github.com/urmi-21/orfipy). Please read the pre-print [here](https://www.biorxiv.org/content/10.1101/2020.10.20.348052v1).

**This research is funded by National Science Foundation grant IOS 1546858, Orphan Genes: An Untapped Genetic Reservoir of Novel Traits, and by the Center for Metabolic Biology, Iowa State University**



## Past Projects

coming soon...











