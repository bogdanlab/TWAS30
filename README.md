TWAS30
======
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

Traits
------
We use the following shorthand notation for the 30 complex traits,

| Shortname | Trait |
|-----|--------------|
| BMI | [Body Mass Index][1] |
| HEIGHT | [Height][2] |
| HB | [Haemoglobin][3] |
| MCH | [Mean Cell Haemoglobin][3] |
| MCHC | [MCH Concentration][3] |
| MCV | [Mean Cell Volume][3] |
| PCV | [Packed Cell Volume][3] |
| RBC | [Red Blood Cell Count][3] |
| PLT | [Number of Platelets][4] |
| FG | [Fasting Glucose][5] |
| FI | [Fasting Insulin][5] |
| HOMA-B | [HOMA-B][5] |
| HOMA-IR | [HOMA-IR][5] |
| HBA1C | [HBA1C][6] |
| HDL | [High Density Lipoprotein][7] |
| LDL | [Low Density Lipoprotein][7] |
| TG | [Triglycerides][7] |
| TC | [Total Cholesterol][7] |
| EY | [Education Years][8] |
| COL | [College][8] |
| FA | [Forearm BMD][9] |
| FN | [Femoral Neck BMD][9] |
| LS | [Lumbar Spine][9] |
| AM | [Age at Menarche][10] |
| RA | [Rheumatoid Arthritis][11] |
| SCZ | [Schizophrenia][12] |
| CD | [Crohn's Disease][13] |
| IBD | [Inflammatory Bowel Disease][13] |
| UC | [Ulcerative Colitis][13] |
| T2D | [Type 2 Diabetes][14] |

Gene Expression
---------------
Similarly, the gene expression study panels used to train models are

| Shortname | Expression Study |
| --------- | ----- |
| CMC | [Commonmind consortium][15] |
| GTEX | [Genotype-Tissue Expression Consortium][16] |
| MET | [Metabolic Syndrome in Men Study (METSIM)][17] |
| NTR | [National Twins Registry][18] |
| YFS | [Cardiovascular Risk in Young Finns Study][19] |

Software and support
--------------------
To compute the genetic correlation of two traits using estimated effects of gene expression, please see [RHOGE](http://github.com/bogdanlab/RHOGE).

For performing TWAS using summary-data, computing expression weights using custom expression panels, and additional post-TWAS analyses please see [FUSION](http://github.com/gusevlab/fusion_twas).

If you have any questions or comments please contact nmancuso@mednet.ucla.edu

[1]: http://www.nature.com/nature/journal/v518/n7538/abs/nature14177.html
[2]: http://www.nature.com/ng/journal/v46/n11/abs/ng.3097.html
[3]: http://www.nature.com/nature/journal/v492/n7429/full/nature11677.html
[4]: http://www.nature.com/nature/journal/v480/n7376/full/nature10659.html
[5]: http://www.nature.com/ng/journal/v42/n2/abs/ng.520.html
[6]: http://diabetes.diabetesjournals.org/content/59/12/3229.long
[7]: http://www.nature.com/ng/journal/v45/n11/full/ng.2797.html
[8]: http://science.sciencemag.org/content/340/6139/1467
[9]: http://www.nature.com/nature/journal/v526/n7571/full/nature14878.html
[10]: http://www.nature.com/nature/journal/v514/n7520/full/nature13545.html
[11]: http://www.nature.com/nature/journal/v506/n7488/full/nature12873.html
[12]: http://www.nature.com/nature/journal/v511/n7510/full/nature13595.html
[13]: http://www.nature.com/ng/journal/v47/n9/full/ng.3359.html
[14]: http://www.nature.com/ng/journal/v44/n9/full/ng.2383.html
[15]: http://www.commonmind.org
[16]: http://www.gtexportal.org/home/
[17]: http://www.jlr.org/cgi/pmidlookup?view=long&pmid=28119442
[18]: http://www.nationalbiobanks.fi/index.php/studies2/30-finnish-twin-cohort
[19]: http://youngfinnsstudy.utu.fi/

