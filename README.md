README: R Section - Advanced Bioinformatics 2025 Assessment

This README provides instructions for the R analysis section (Sections 3.1–3.19) of the Advanced Bioinformatics assessment. It explains the file structure, dependencies, and how to render and use the R Markdown report.

Files

assessment_2025.RmdThe R Markdown source file. Contains all code chunks and narrative for Sections 3.1–3.19.

assessment_2025.htmlThe knitted HTML output for easy review of code, results, and figures.

counts.csvRaw counts matrix for RNA-seq (genes × samples).

exercise1_sample_description.infoSample metadata table (rows = samples, includes condition and batch).

DE_results_KOa_vs_FFa.csvFull differential-expression results (shrunken log2FC) for KOa vs FFa.

mycmelrep1_peaks.xls, mycmelrep2_peaks.xlsMACS2 output files for ChIP-seq replicates.

top500_common_peaks.faFASTA file of the top 500 common peaks (200 bp), used for MEME-ChIP.

Dependencies

Required R packages (automatically installed by the setup chunk):

tidyverse

DESeq2

pheatmap

GenomicRanges

ChIPseeker

BSgenome.Hsapiens.UCSC.hg19

genefilter

readxl

These packages are installed and loaded at the beginning of the .Rmd.

Rendering the Report

Open assessment_2025.Rproj in RStudio.

Ensure all data files are in the project directory (same folder as the .Rmd).

Click the Knit button or run:

rmarkdown::render("assessment_2025.Rmd")

Inspect assessment_2025.html for code output, plots, and tables.

Sections Overview

3.1–3.7: Basic R tasks (sum, functions, loops, plots with mtcars and cars).

3.8–3.15: RNA-seq analysis with DESeq2 (data import, transformations, PCA, heatmaps, DE results).

3.16–3.19: ChIP-seq mini-analysis (peak intersection, ranking, resizing, sequence extraction, MEME-ChIP motif table).

Notes

The HTML output includes all figures and tables inline for easy review.

The full DE results CSV can be used for additional annotation or downstream analysis.

The FASTA file top500_common_peaks.fa was uploaded to MEME-ChIP; motif summaries are in Section 3.19 of the report.
