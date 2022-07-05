# Resistance_in_Acinetobacter-Baumanii

The purpose of this repository is to replicate the study, 'Schultz MB, Pham Thanh D, Tran Do Hoan N, et al. Repeated local emergence of carbapenem-resistant Acinetobacter baumannii in a single hospital ward. Microb Genom. 2016;2(3):e000050. Published 2016 Mar 2. doi:10.1099/mgen.0.000050" for non-publication reasons using bioinformatics tools taught during my genomics course with HackBio.

The aim of the paper was to understand, identify and study the population and/or emergence of imipenem-resistant A.baumanii and investigate their phylogenetic relationship to the imipenem-susceptible type, all isolated from the same hospital ward but at different periods of time.

# Methodology

 1. From the collected isolates, DNA was extracted and sequenced using the Wizard Genomic Extraction kit (Promega) and 96-plex bar-coded 100bp paired end sequencing via illumina    HiSeq 2500 respectively. This resulted to a total of 147 genomes for analysis that are made available in the European Nucleotide Archive under the project ERP001080. The reads obtained were mapped against the Acinetobacter baumannii MDR-ZJ06, complete genome with the GenBank accession number of CP001937.2

 2. From the SRA-NCBI, I opt to use only 20 genomes reads to retrieve the NGS data
	- download sratools-kit 2.10.9
	- using the ,/prefetch command
	- convert each SRA file to fastq format using the command, ./fastq-dump --split files ".sra"
 
 3. Quality control using fastp command,fastp --in1 *_1.fastq --in2 *_2.fastq --out1 *_1_trimmed.fastq --out2 *_2_trimmed.fastq -l 30 -h *.html &> *.log
 included the following,
	- Adapter trimming
	- Quality trimming
	- Quality assessment

 4. For the read mapping and alignment to the reference genome, using the following bioinformatics tools
      - BWA


