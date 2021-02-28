---
layout: post
title:  "Current top commands"

---

I recently got in touch with a future colleague who was keen on learn more about genomics and that got me thinking about commands I frequently use these days. I've previously touched upon the usefulness of [github](https://emelinefavreau.github.io/2020/09/30/using-github.html). So here are more snapshots of my bioinformatics workbench.

![uk spring flowers on green grass](/assets/2021-02-spring-flowers.jpg)

_February 2021: Spring is coming while the pandemic has us in lockdown still_


**Project organisation**. Genomic datasets are huge and my work space does not allow for many of these files of several mega or giga bytes. I cannot keep multiple copies of each dataset in my projects, because my work space would be full. Instead, I give each project an access to the archived copy via a soft-linked version of the dataset (e.g. ln -s archive/my-sequences.fasta project1/input/my-sequences.fasta). The syntax of my command line will be as expected (e.g. head project1/input/my-sequences.fasta), the tools will use the dataset as expected, and my work space remains clutter-free. Try it by typing *man ln* in your terminal.

**Well-planned experiments**. Some genomic experiments can take several hours, which makes me more aware of good time management. One good practice that I learnt from wet lab is to set the experiment in a lab room before lunch (say, a PCR), walk away from that room for a well-earned break, and come back in the afternoon to check the result. I do the same with the *in silico* experiments. From my work space, I enter my project space where datasets and tools are at the ready. I "create a lab room" and start the experiment, check for a minute that everything is running as expected, I then "walk away from the room" without the experiment stopping. I can "re-enter the room" as I wish to check the workflow, and I once the results are in, I can "remove the room". Make your own lab rooms with *screen* or *tmux*.

**Speed things up with parallel**. One of the common tasks on my work bench is to map sequenced reads to a genome assembly. It is the process to match the sequences of nucleotides between the two sets of data: many small sequences that came out of a sequencer (reads) and a small number of long sequences that came out of an assembling algorithm (genome). This can take several hours, even days! I recently had a hundred samples to map to the assembly. To speed up the process, I used a tool that uses multiple computers at once, with the same output as if I was to run the tasks sequentially, one sample at a time. Learn more about [GNU parallel](https://www.gnu.org/software/parallel/parallel_cheat.pdf).

I am also using R ggplot, Nextlow, Git push. I'll talk about these another time.
