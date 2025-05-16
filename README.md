# Gene Expression Analysis of Liver and Pancreas Cells Using scRNA-seq Data
Comparative single-cell RNA-seq analysis of liver and pancreas tissues to identify gene expression differences related to metabolism and hormone production.
## Objective
The liver and pancreas are essential organs with distinct but interrelated functions: the liver primarily manages metabolism, while the pancreas regulates hormone production, particularly insulin and glucagon. Understanding the gene expression profiles unique to these tissues at a single-cell level can provide insights into their specialized roles and inform disease research and targeted therapies.
## Data
The dataset used for this analysis is the Tabula Muris project, which includes single-cell RNA sequencing data from approximately 100,000 cells across 20 mouse organs and tissues, including the liver and pancreas. Metadata such as tissue type, sub-tissue, mouse sex, and cell sorting method are included, enabling detailed comparative analysis.
## Data Processing 
- **Filtering**: Cells with extreme library sizes and genes with low expression were removed to reduce noise and bias.
- **Normalization and Transformation**: Counts were normalized to adjust for sequencing depth, and a square root transformation was applied to stabilize variance across cells.
## Dimensionality Reduction and Clustering
- **Principal Component Analysis (PCA)**: Used for initial reduction of high-dimensional gene expression data to identify main sources of variation between liver and pancreas cells.
- **UMAP**: Applied for enhanced visualization of cell clusters, highlighting finer tissue-specific distinctions.
- **K-means Clustering**: Selected to group cells into distinct clusters based on gene expression profiles, effectively separating liver and pancreas populations and their subtissues.
## Differential Expression Analysis 
A comparative analysis was performed to identify genes significantly upregulated or downregulated in liver vs. pancreas cell populations. Genes analyzed include ALB, TTR (liver-associated), INS1, and GCG (pancreas-associated), among others.
## Key Findings
- Liver cells show strong expression of metabolic genes such as ALB and TTR.
- Pancreas cells exhibit high expression of hormone-related genes, including INS1 and GCG.
- Clustering and dimensionality reduction reveal distinct cell populations corresponding to liver and pancreas tissues and their subtissues.
- The results highlight the complementary metabolic and endocrine roles of liver and pancreas cells.
## Future Directions
- **Human Data Integration**: Incorporating human scRNA-seq datasets could increase clinical relevance.
- **Advanced Clustering**: Applying more sophisticated clustering or machine learning techniques may reveal finer cell type distinctions.
- **Longitudinal Studies**: Investigating gene expression changes over time to understand disease progression or development.
- **Experimental Validation**: Testing the functional roles of key genes through experimental studies.
