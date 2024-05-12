re-annotation  
First, we align the probes from probemain and the sequences of genes in Homo_sapiens.GRCh38.cdnaANDncrna.fa. We then filter out the probes that only match a single lncRNA.  
  
quantitative 
Then, we quantify the lncRNA based on the correspondence between the probes and lncRNAs, as well as the raw data from the expression microarray (CEL files).  
  
Differential expression analysis 
Afterward, we performed gene differential expression analysis and other related analyses based on the expression level files of lncRNAs in different brain regions.  
  
eQTL analysis file preparation 
Next, we prepared all the files required for eQTL analysis, including the first three PCA files for SNPs, the first fifteen PEER factor files for gene expression data, and information about sample age and sex.
  
eQTL analysis and eQTL permutation 
Afterward, we conducted eQTL analysis and eQTL permutation analysis to explore the degree of association between lncRNA and SNPs. This allowed us to identify lncRNAs that are most influenced by SNPs and SNPs that have the greatest impact on lncRNA expression.  
  
Correlation of cis-eQTL effects between tissues 
Then, we calculated the correlation of cis-eQTL effects between tissues.  
  
PredictDB  
We utilized the code in PredictDB.txt to call other R scripts within the folder and trained gene prediction models for each brain region.  
  
TWAS  
Next, we utilized the TWAS.txt file to invoke the SPrediXcan.py code. By integrating the gene training models with the disease GWAS files, we were able to identify lncRNAs that potentially correlate with the disease.  
  
2SLS analysis
After conducting eQTL analysis on mRNA, we proceeded to perform eQTL analysis on lncRNA and mRNA. Subsequently, we performed a 2SLS analysis on the eQTL results of lncRNA and mRNA to identify the mRNA that is potentially regulated by the lncRNA of interest.  
  
enrichment
Finally, we performed an enrichment analysis on the selected mRNA to explore their functional annotations and potential biological roles. This analysis indirectly revealed the functional implications of the lncRNAs that influence them.  



