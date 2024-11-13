## Project Overview

This project aims to make complex multi-omics data (gene expression, mutation, and copy number variation) more accessible and insightful through data visualization. By applying advanced methods such as heatmaps and Multiple Factor Analysis (MFA), the visualizations help illustrate the distinct molecular profiles of cancer subtypes in colorectal cancer. These methods not only enhance data comprehension but also reveal underlying patterns that may not be evident in raw data alone. While the primary data files (.csv) and certain packages are not included here due to their large size, this README outlines the visualization approach and the code used to generate the analysis.

## Data Visualization Techniques
# 1. Heatmaps
In this project, three heatmaps were created to examine each type of multi-omics data (gene expression, mutation, and copy number variation) individually. Each heatmap provides unique insights into the data, allowing observers to identify subtype-specific patterns and gain a clearer understanding of the molecular differences across cancer subtypes

Gene Expression Heatmap: Visualizes differences in gene expression levels, with each row as a gene and each column as a tumor. Annotations by subtype help show subtype-related expression patterns. By observing clusters in gene expression, we can start to see if certain genes are more actively expressed in specific cancer subtypes. For instance, genes that consistently show higher or lower expression in one subtype might be linked to the biological mechanisms defining that subtype. Observing these patterns helps in identifying subtype-specific gene activity, providing potential targets for further research or therapy.


<img width="300" alt="Screenshot 2024-11-13 at 1 58 07 AM" src="https://github.com/user-attachments/assets/583cb3ab-2b77-400d-baf4-264ea8848257">

Mutation Data Heatmap: Highlights the mutation load across tumors, where clusters align closely with cancer subtypes, particularly showing the hyper-mutated status of some subtypes (e.g., CMS1). Mutation clustering often correlates strongly with subtype. For example, in colorectal cancer, one subtype may show a hyper-mutated status (more mutations across the board), while another may have fewer mutations. By examining the mutation heatmap, it becomes apparent that certain subtypes (e.g., CMS1) have significantly higher mutation rates than others (e.g., CMS3). This difference in mutation load helps distinguish subtypes and may be indicative of different pathways driving tumor progression.


<img width="300" alt="Screenshot 2024-11-13 at 1 58 52 AM" src="https://github.com/user-attachments/assets/43dc24a6-f977-436a-9c33-a7380ed21076">

Copy Number Variation (CNV) Heatmap: Examines amplifications and deletions, providing visual cues on gene copy changes specific to subtypes.The CNV heatmap can reveal subtype-specific patterns of amplification and deletion, which may contribute to tumor behavior. For example, if a particular subtype consistently shows amplifications in oncogenes or deletions in tumor suppressor genes, it suggests distinct mechanisms underlying tumor growth and survival in that subtype. Observing these patterns provides insights into genetic vulnerabilities that could be targeted in subtype-specific therapies.


<img width="300" alt="Screenshot 2024-11-13 at 1 59 50 AM" src="https://github.com/user-attachments/assets/01c7bd2e-8dee-4f9d-affb-3c3b2f57d33c">

# 2 Multiple Factor Analysis (MFA)
 MFA combines all omics data types into a single reduced-dimensional space, creating a two-dimensional scatter plot that visually separates the cancer subtypes. This method provides a simplified but comprehensive view of the data by condensing numerous features into just a few factors, aiding in distinguishing between molecular characteristics unique to each subtype. For example, if CMS1 and CMS3 tumors naturally separate into distinct clusters in the MFA scatter plot, this confirms that the differences seen in individual heatmaps (such as high mutation load in CMS1) are part of an underlying molecular signature that consistently differentiates subtypes.


<img width="300" alt="Screenshot 2024-11-13 at 2 01 24 AM" src="https://github.com/user-attachments/assets/b1bae966-8942-492e-8f75-77ffa9f26bb4">


# 3 Future Implementations


In future updates, this analysis will be expanded with:

Non-negative Matrix Factorization (NMF): To further break down complex datasets into interpretable patterns and reveal hidden structures across samples.
K-means Clustering: To enhance clustering of tumor samples, adding another layer of subtype distinction and possibly validating MFA clusters with another clustering method.

