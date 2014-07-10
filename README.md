DrosophilaPopGenData-Rogers2014
===============================

Population Genetic Data for *Drosophila yakuba* and *Drosophila simulans*.

Residual poly tracts
================================
To detect regions of residual heterozygosity, we called
SNPs using samtools under a diploid model. Segments with residual heterozygosity were detected
using an HMM (HMM;http://cran.r-project.org/web/.  The most likely path was calculated using the Viterbi
algorithm, and heterozygous segments 10 kb or larger were retained. Heterozygous blocks
within 100kb of one another in a sample strain were clustered together as a single segment
to define the span of residual heterozygosity within inbred lines.  

Further description is available in Rogers et al. 2014.


SNP VCF files are available at http://molpopgen.org/Data


Theta
===============================
We estimate Theta_pi, Theta_W, and Tajima's D for all SNPs in the D. yakuba and D. simulans genomes,
removing sites with missing or ambiguous data as well as heterozygous sites. We calculate:

* Window Midpoint
* the number of sites with coverage sufficient to assay SNPs
* Theta_pi,
* Theta_W 
* Tajima's D 

Estimates provided are for 5 kb windows moving in a 500 bp slide across the genome.   Positions in each file designate the window midpoint.  Population genetic parameters were calculated using libsequence module for C++ (Thornton, K. 2003).  We exclude all sites with missing data, ambiguous sequence, or heterozygous sites.


Cite
===============================
Rogers et al. 2014  Tandem duplications and the limits of natural selection in Drosophila yakuba and Drosophila simulans.  http://arxiv.org/abs/1405.0518

