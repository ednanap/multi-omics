# Project Overview

This project aims to make complex multi-omics data (gene expression, mutation, and copy number variation) more accessible and insightful through data visualization. By applying advanced methods such as heatmaps and Multiple Factor Analysis (MFA), the visualizations help illustrate the distinct molecular profiles of cancer subtypes in colorectal cancer. These methods not only enhance data comprehension but also reveal underlying patterns that may not be evident in raw data alone. While the primary data files (.csv) and certain packages are not included here due to their large size, this README outlines the visualization approach and the code used to generate the analysis.

# Data Visualization Techniques
# 1. Heatmaps: Heatmaps provide a powerful way to examine each data type independently:
Gene Expression Heatmap: Visualizes differences in gene expression levels, with each row as a gene and each column as a tumor. Annotations by subtype help show subtype-related expression patterns.
<img width="300" alt="Screenshot 2024-11-13 at 1 58 07 AM" src="https://github.com/user-attachments/assets/583cb3ab-2b77-400d-baf4-264ea8848257">

Mutation Data Heatmap: Highlights the mutation load across tumors, where clusters align closely with cancer subtypes, particularly showing the hyper-mutated status of some subtypes (e.g., CMS1).

<img width="300" alt="Screenshot 2024-11-13 at 1 58 52 AM" src="https://github.com/user-attachments/assets/43dc24a6-f977-436a-9c33-a7380ed21076">

Copy Number Variation (CNV) Heatmap: Examines amplifications and deletions, providing visual cues on gene copy changes specific to subtypes.
<img width="300" alt="Screenshot 2024-11-13 at 1 59 50 AM" src="https://github.com/user-attachments/assets/01c7bd2e-8dee-4f9d-affb-3c3b2f57d33c">
# 2 Multiple Factor Analysis (MFA)
 MFA combines all omics data types into a single reduced-dimensional space, creating a two-dimensional scatter plot that visually separates the cancer subtypes. This method provides a simplified but comprehensive view of the data by condensing numerous features into just a few factors, aiding in distinguishing between molecular characteristics unique to each subtype.

<img width="300" alt="Screenshot 2024-11-13 at 2 01 24 AM" src="https://github.com/user-attachments/assets/b1bae966-8942-492e-8f75-77ffa9f26bb4">


