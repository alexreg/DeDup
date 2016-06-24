# DeDup
A merged read deduplication tool capable to perform merged read deduplication on single end data. 

Author: Alexander Peltzer <alexander.peltzer@uni-tuebingen.de>

###### Method
The DeDup tool is designed to work with forward, reverse and merged reads (forward and reverse combined to make a single read).
DeDup expects the different kinds of reads to have read names that begin with one of the following prefixes:

- F_
- R_
- M_

To remove PCR duplicates we only retain a single read for a given genomic position and read direction. For M_ (merged) reads we know both the start and end of the sequenced fragment. For F_ and R_ reads we only know the start or end of the sequenced fragment becuase the read length is variable.

 
