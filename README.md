TWAS30
------
This repository contains transcriptome-wide association study (TWAS) summary statistics for the
30 traits reported in

**Integrating gene expression with summary association statistics to
identify susceptibility genes for 30 complex traits**.,
Nicholas Mancuso, Huwenbo Shi, Pagé Goddard, Gleb Kichaev,
Alexander Gusev, Bogdan Pasaniuc.
American Journal of Human Genetics. 2017 Feb. [doi: 10.1016/j.ajhg.2017.01.031](http://www.cell.com/ajhg/fulltext/S0002-9297(17)30032-0)

Each `*.txt` file contains the TWAS results for a particular trait. Each file is prefixed with a header naming the 12 columns.
A description of each of these columns is provided below,

| Column | Description |
| ------ | ----------- |
| TRAIT | GWAS trait |
| GENE | Gene or transcript used to test for association with GWAS trait |
| CHR | Chromosome the gene is located on |
| TxS | Transcription start site |
| TxE | Transcription end site |
| STUDY | The original panel expression levels were measured in |
| TWAS.Z | TWAS association statistic |
| TWAS.P | TWAS association p-value |
| BEST.GWAS.RSID | RSID of the best GWAS SNP within 1 Mb of the gene TxS (i.e. smallest p-value) |
| BEST.GWAS.P | P-value of the best GWAS SNP |
| GWAS.HSQ.LOCAL | Local heritability estimate of GWAS trait |
| ALPHA | Standardized effect of gene/transcript expression on trait |

We use the following shorthand notation for the 30 complex traits,

| Shortname | Trait |
|-----|--------------|
| BMI | Body Mass Index |
| HEIGHT | Height |
| HB | Haemoglobin |
| MCH | Mean Cell Haemoglobin |
| MCHC | MCH Concentration |
| MCV | Mean Cell Volume |
| PCV | Packed Cell Volume |
| RBC | Red Blood Cell Count |
| PLT | Number of Platelets |
| FG | Fasting Glucose |
| FI | Fasting Insulin |
| HBA1C | HBA1C |
| HOMA-B | HOMA-B |
| HOMA-IR | HOMA-IR |
| HDL | High Density Lipoprotein |
| LDL | Low Density Lipoprotein |
| TC | Total Cholesterol |
| TG | Triglycerides |
| EY | Education Years |
| COL | College |
| FA | Forearm BMD |
| FN | Femoral Neck BMD |
| LS | Lumbar Spine |
| AM | Age at Menarche |
| RA | Rheumatoid Arthritis |
| SCZ | Schizophrenia |
| CD | Crohn's Disease |
| IBD | Inflammatory Bowel Disease |
| UC | Ulcerative Colitis |
| T2D | Type 2 Diabetes |


To compute the genetic correlation of two traits using estimated effects of gene expression, please see [RHOGE](http://github.com/bogdanlab/RHOGE).

For performing TWAS using summary-data, computing expression weights using custom expression panels, and additional post-TWAS analyses please see [FUSION](http://github.com/gusevlab/fusion_twas).

If you have any questions or comments please contact nmancuso@mednet.ucla.edu
