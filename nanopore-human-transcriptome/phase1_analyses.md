This page contains brief information and files from the consortium analysis.
### Performance measurements
We calculated sequencing statistics using [marginStats](https://github.com/benedictpaten/marginAlign) on alignment of native RNA and cDNA reads to gencode.v27.transcripts.fa using minimap2 (_-ax map-ont_) mode. We created a summary of unique genes and isoforms detecte by native RNA sequence data upon alignments fo the GENCODE v27 reference sequence set. Additionally, we calculated 5mers in sequence data relative to FLAIR high-confidence reference isoforms. 

 - [Genes and Isoforms detected](http://s3.amazonaws.com/nanopore-human-wgs/rna/phase1_analyses/Supplementary_Tables_Sx.Native_RNA_genes_isoforms_GENCODEv27.xlsx)
 - [Kmer counts](http://s3.amazonaws.com/nanopore-human-wgs/rna/phase1_analyses/Supplementary_Tables_S1_S2_kmer_counts_nativeRNA_cDNA.xlsx)
 
### FLAIR isoforms
We used the gencode.v27.transcripts.fa to align the pass native RNA and pass cDNA reads.  
Isoforms defined from FLAIR v1.1 are in [PSL format](https://genome.ucsc.edu/FAQ/FAQformat.html#format2). From the native RNA data, we generated two sets of isoforms: set A and set B. Set A contains all isoforms (71,899 isoforms) from default FLAIR output with a minimum of 5 supporting reads, as described in the Online Methods. Set B (50,039 isoforms) is a more stringent set of nvRNA isoforms than set A. To generate set B, set A isoforms that are subsets of longer set A isoforms are removed and only the longest isoform of each unique splice junction chain is retained. We also have a set of FLAIR isoforms defined from cDNA data (99,574 isoforms).

 - [nvrna.flair.isoforms.setA.psl](http://s3.amazonaws.com/nanopore-human-wgs/rna/phase1_analyses/nvrna.flair.isoforms.setA.psl)
 - [nvrna.flair.isoforms.setB.psl](http://s3.amazonaws.com/nanopore-human-wgs/rna/phase1_analyses/nvrna.flair.isoforms.setB.psl)
 - [cdna.flair.isoforms.psl](http://s3.amazonaws.com/nanopore-human-wgs/rna/phase1_analyses/cdna.flair.isoforms.psl)
 
### Poly(A) calls

### Nanopolish indexes for signal analyses
