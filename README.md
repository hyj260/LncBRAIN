1-re-annotation.txt  
First, we align the probes from probemain and the sequences of genes in Homo_sapiens.GRCh38.cdnaANDncrna.fa. We then filter out the probes that only match a single lncRNA.  
  
2-quantitative.txt  
Then, we quantify the lncRNA based on the correspondence between the probes and lncRNAs, as well as the raw data from the expression microarray (CEL files).  
  
3-Differential_expression_analysis.txt  
Afterward, we performed gene differential expression analysis and other related analyses based on the expression level files of lncRNAs in different brain regions.  
  
4-eQTL_analysis_file_preparation.txt  
Next, we prepared all the files required for eQTL analysis, including the first three PCA files for SNPs, the first fifteen PEER factor files for gene expression data, and information about sample age and sex.
  
5-eQTL_analysis.txt and 6-eQTL_permutation.txt  
Afterward, we conducted eQTL analysis and eQTL permutation analysis to explore the degree of association between lncRNA and SNPs. This allowed us to identify lncRNAs that are most influenced by SNPs and SNPs that have the greatest impact on lncRNA expression.  
  
7-Correlation_of_cis-eQTL_effects_between_tissues.txt  
Then, we calculated the correlation of cis-eQTL effects between tissues.  
  
8-PredictDB  
We utilized the code in PredictDB.txt to call other R scripts within the folder and trained gene prediction models for each brain region.  
  
9-TWAS  
Next, we utilized the TWAS.txt file to invoke the SPrediXcan.py code. By integrating the gene training models with the disease GWAS files, we were able to identify lncRNAs that potentially correlate with the disease.  
  
10-2SLS_analysis.txt  
After conducting eQTL analysis on mRNA, we proceeded to perform eQTL analysis on lncRNA and mRNA. Subsequently, we performed a 2SLS analysis on the eQTL results of lncRNA and mRNA to identify the mRNA that is potentially regulated by the lncRNA of interest.  
  
11-enrichment.txt  
Finally, we performed an enrichment analysis on the selected mRNA to explore their functional annotations and potential biological roles. This analysis indirectly revealed the functional implications of the lncRNAs that influence them.  



