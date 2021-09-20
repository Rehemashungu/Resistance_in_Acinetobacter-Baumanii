# Resistance_in_Acinetobacter-Baumanii

The purpose of this repository is to replicate the study, 'Schultz MB, Pham Thanh D, Tran Do Hoan N, et al. Repeated local emergence of carbapenem-resistant Acinetobacter baumannii in a single hospital ward. Microb Genom. 2016;2(3):e000050. Published 2016 Mar 2. doi:10.1099/mgen.0.000050" for non-publication reasons using bioinformatics tools taught during my genomics course with HackBio.

The aim of the paper was to understand, identify and study the population and/or emergence of imipenem-resistant A.baumanii and investigate their phylogenetic relationship to the imipenem-susceptible type, all isolated from the same hospital ward but at different periods of time.

# Methodology

 1. From the collected isolates, DNA was extracted and sequenced using the Wizard Genomic Extraction kit (Promega) and 96-plex bar-coded 100bp paired end sequencing via illumina HiSeq 2500 respectively. This resulted to a total of 147 genomes for analysis that are made available in the European Nucleotide Archive under the project ERP001080. 
The reads obtained were mapped against the 3 940 614 reference genome of A.baumanii GC2 strain 1656-2 with the GenBank accession number of CP001921.1)

 2. From the ENA, I opt to use only 10 genomes reads

 3. For the mapping and alignment to the reference genome, i will use the following pipeline.
      - The Burrows-Wheeler Transform
      - Bowtie2
      - SAMtools


