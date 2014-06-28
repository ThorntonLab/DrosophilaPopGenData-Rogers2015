DrosophilaPopGenData-Rogers2014
===============================

Population Genetic Data and SNPs for Drosophila yakuba and Drosophila simulans

Theta per site for 10 kb windows with a 1 kb slide by chromosome.  Population genetic parameters were calculated using libsequence module for C++ (Thornton, K. 2003).  We exclude all sites with missing data, ambiguous sequence, or heterozygous sites.

Residual poly tracts
================================
To detect regions of residual heterozygosity, we called
SNPs using samtools under a diploid model. Segments with residual heterozygosity were detected
using an HMM (HMM;http://cran.r-project.org/web/.  The most likely path was calculated using the Viterbi
algorithm, and heterozygous segments 10kb or larger were retained. Heterozygous blocks
within 100kb of one another in a sample strain were clustered together as a single segment
to dene the span of residual heterozygosity within inbred lines.  

Further description is available in Rogers et al. 2014.


SNP VCF files are available at http://molpopgen.org/Data


Theta
===============================
We estimate Theta_pi, Theta_W, and Tajima's D for all SNPs in the D. yakuba and D. simulans genomes,
removing sites with missing or ambiguous data as well as heterozygous sites. We calculate Theta_pi,
Theta_W, and Tajima's D for 10 kb windows moving in a 1kb slide across the genome


Format
=====
WindowMidpoint ThetaPi ThetaW TajimasD



Cite
===============================
Rogers et al. 2014  Tandem duplications and the limits of natural selection in Drosophila yakuba and Drosophila simulans.  http://arxiv.org/abs/1405.0518

