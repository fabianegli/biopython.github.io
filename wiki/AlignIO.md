---
title: AlignIO
permalink: wiki/AlignIO
layout: wiki
---

This page describes Bio.AlignIO, a new multiple sequence Alignment
Input/Output interface for BioPython which is currently only in our
source code repository. It should be included in the next release of
Biopython.

You may already be familiar with the [Bio.SeqIO](SeqIO "wikilink")
module which deals with files containing one or more sequences
represented as [SeqRecord](SeqRecord "wikilink") objects. Similarly,
Bio.AlignIO deals with files containing one or more sequence alignments
represented as Alignment objects. The same set of functions is provided
for input and output.