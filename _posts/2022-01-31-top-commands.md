---
layout: post
title:  "Top Command Lines"

---

I welcomed a new colleague this week on campus, this was awesome after several months of working from home! Cintia Oi is coming with fantastic ideas and questions to challenge some genomic data. I'm updating my "current top commands" to share more of what's going on my screen.

**Writing reproducible science**. In our lab, Chris Wyatt is the torchbearer of [Nextlow](https://www.nextflow.io/) and is encouraging us to use this version-control, open-source workflow pipeline. This allowed me to clean raw RNAseq data, to run QC steps, to map reads to a genome, to obtain read counts ready for statistical analyses. The process was relatively straight forward: select on a platform the workflow (e.g. https://nf-co.re/rnaseq/1.3), download an image containing the recipe for the workflow on your cluster, set the experiment, and let it run in the background. It can be used for all sizes of data, so I could run it with all sorts of samples laying around in our lab. Enrich your science with reproducibility: https://nf-co.re/usage/nextflow (tutorials).

**Explaining results visually**. Once the data have been analysed, I like to plot them to assess whether the starting hypothesis stands the test. I can spend many happy hours building a pretty graph, usually using R ggplot2 and looking for inspiration on this [gallery](https://www.r-graph-gallery.com/). The code is avaiable for each graph, making my life easier. I pick colours that will convey the take-home message best, and that are colour-blind friendly (https://colorbrewer2.org/). Teach yourself some neat visualization tricks: https://datacarpentry.org/R-ecology-lesson/04-visualization-ggplot2.html

**Backing up your work**. Once all is coded, statistical tests and data visualisation, I make sure to secure all scripts and READMEs. This is important because I might not look at the data for a long time, so leaving my desk tidy is more efficient in the long term. This is important because my laptop could cease to exist, and all efforts and outputs with it. And this is not cool! So I regularly practice git push, a simple command that mirrors my laptop's content with a Github remote repo. Some colleagues practice the "plug the external hard drive and copy files" system. This is good too. Anything is better than just leaving your script on your laptop. Practice it here: https://swcarpentry.github.io/git-novice/ 

I am also using Python scikit-learn, Docker, qsub. I’ll talk about these another time.