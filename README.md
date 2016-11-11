metaPGAP
========

metaPGAP is a pipeline for building core genome using PAN genome approach. This pipeline takes complete or draft genome assemblies and perform annotation using Prokka. The Prokka predictions then used to build core genome using get_homologues tool. For core genes phylogeny Mafft and RaXML used.

Full list of required softwares and dependencies:

metaPGAP steps:
--------------------
(1). Download data from https://github.com/mitul-patel/data/archive/master.zip
(2). Genome Annotation using Prokka
(3). PAN genome analysis using get_homologues: BDBH, COG and OMCL
(4). Multiple sequence alignment of CORE genes
(5). Phylogenetic analysis of CORE genes using RaXML
(6). Visualization of phylogenetic tree using Newick tools

metaPGAP requirements:
-----------------------------
Python (http://python.org)
BioPython (1.5 or higher) with NumPy (http://biopython.org/wiki/Download)
Prokka (https://github.com/tseemann/prokka)
get_homologues (https://github.com/eead-csic-compbio/get_homologues)
Mafft (http://mafft.cbrc.jp/alignment/software/)
Perl (http://Perl.org)
AMAS (https://github.com/marekborowiec/AMAS)
RaXML (https://github.com/stamatak/standard-RAxML)
Newick tools (http://cegg.unige.ch/newick_utils)



General Use
--------------
Usage:

Docker PULL Command:

     docker pull mitulpatel/metapgap     

Docker RUN Command:

      docker run -v `pwd`:/metaPGAP -w /metaPGAP mitulpatel/metapgap

