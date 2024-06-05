# Probe set re-annotation  
First, the probes were align from probemain and the sequences of genes in Homo_sapiens.GRCh38.cdnaANDncrna.fa. We then filter out the probes that only match a single lncRNA.  
  
# Quantification of lncRNAs  
Then, the lncRNAs were quantified based on the correspondence between the probes and lncRNAs, as well as the raw data from the expression microarray (CEL files).  
  
# Differential expression analysis  
Afterward, the elncRNA differential expression analysis and other related analyses were performed based on the expression level files of lncRNAs in different brain regions.  
  
# eQTL analysis and permutation  
Next, we prepared all the files required for eQTL analysis, including the first three PCA files for SNPs, the first fifteen PEER factor files for gene expression data, and information about sample age and sex. Afterward, we conducted eQTL analysis and eQTL permutation analysis to explore the degree of association between lncRNA and SNPs. This allowed us to identify lncRNAs that are most influenced by SNPs and SNPs that have the greatest impact on lncRNA expression.  
  
# Correlation of cis-eQTL effects between tissues  
Then, we calculated the correlation (rb) to compare the similarity of of cis-eQTL effects on lncRNA expression between two of the ten brain regions. It is an unbiased correlation estimate of eQTL effects, which accounts for both effect strength (beta values) and significance (errors or P values) in this process.
  
# PredictDB establishment
We utilized the code in PredictDB.txt to call other R scripts within the folder and trained gene prediction models for each brain region.  
  
# TWAS analysis
Next, we utilized the TWAS.txt file to invoke the SPrediXcan.py code. By integrating the gene training models with the disease GWAS files, we were able to identify lncRNAs that potentially correlate with the disease.  
  
# 2SLS analysis  
After conducting eQTL analysis on mRNA, we proceeded to perform eQTL analysis on lncRNA and mRNA. Subsequently, the 2SLS analysis was performed on the eQTL results of lncRNA and mRNA to identify the mRNA that is potentially regulated by the lncRNA of interest.  
  
# Enrichment analysis
Finally, we performed an enrichment analysis on the selected mRNA to explore their functional annotations and potential biological roles. This analysis indirectly revealed the functional implications of the lncRNAs that influence them.  



