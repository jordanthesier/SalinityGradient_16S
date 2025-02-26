# fastqc

## Full Path: export PATH=/programs/FastQC-0.12.1:$PATH

/workdir/<your_netID>/Salinity_Gradient16S/data/01_DADA2/01_raw_gzipped_fastqs/*.fastq.gz \
	--threads 5 \
	-o /workdir/<your_netID>/Salinity_Gradient16S/analysis/00_FastQC/fastqc_reports/

# multiqc

## Full Path: export PYTHONPATH=/programs/multiqc-1.15/lib64/python3.9/site-packages:/programs/multiqc-1.15/lib/python3.9/site-packages
export PATH=/programs/multiqc-1.15/bin:$PATH

multiqc fastqc_reports/ -o multiqc_results/

