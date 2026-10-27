# 🧬 RNA-seq Analysis | Understanding Heart Disease Through Gene Expression

### 🌐 [Explore My Live Project Website](https://vmadagiri.github.io/CardioSeq/)

**R • Bioinformatics • Data Analysis • Data Visualization**

## 💗 Why I Built This

I've always been interested in how biology and programming can work together to answer questions we can't easily answer just by looking at the data.

For this project, my team and I wanted to understand what happens at the gene-expression level in people with **dilated cardiomyopathy (DCM)**, a condition that causes the heart to become enlarged and makes it harder to pump blood.

We were especially curious about whether gene expression patterns differ between male and female patients.

Instead of just looking at individual genes, we wanted to explore the bigger picture and see which biological pathways might be involved.

## 🎯 Our Research Question

**How does gene expression differ between patients with DCM and people without heart failure, and are there differences between male and female patients?**

Our hypothesis was that DCM would be associated with changes in genes involved in inflammation and heart remodeling, with some differences between males and females.

## 📊 The Dataset

We used a real, publicly available RNA-seq dataset from the **MAGNet consortium**, which contains gene-expression data from human heart tissue.

**Dataset:** [GSE141910 — NCBI Gene Expression Omnibus](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE141910)

| Group | Samples |
|---|---:|
| Non-failing hearts | 152 |
| DCM hearts | 153 |
| **Total** | **305** |

The dataset allowed us to compare gene-expression patterns between healthy donor hearts and hearts affected by DCM, including comparisons between male and female samples.

## 🛠️ How We Analyzed the Data

We used R to clean, process and visualize the RNA-seq data.

Our workflow included:

- Filtering genes with very low expression
- Transforming the data to make comparisons easier
- Using **PCA and UMAP** to explore patterns between samples
- Creating **volcano plots** to identify gene-expression differences
- Comparing male and female samples
- Using **KEGG pathway analysis** to explore the biological processes associated with those differences

The biggest goal was to connect what we saw in our graphs back to actual biological questions.

## 📈 Visualizations

Here are some of the graphs we created while exploring the data.

### 1. PCA Analysis

PCA helped us see how samples compared based on their overall gene-expression patterns.

![PCA Analysis](https://github.com/user-attachments/assets/57057b5e-1f44-4a9c-82cc-851477eac122)

### 2. UMAP Analysis

We used UMAP to explore how samples grouped together and whether there were noticeable patterns between different patient groups.

![UMAP Analysis](https://github.com/user-attachments/assets/6d7b422a-15db-481b-9550-0d09f0ed4262)

### 3. Gene Expression: Female vs. Male DCM

This volcano plot compares gene-expression differences between female and male patients with DCM.

![Female vs Male DCM Volcano Plot](https://github.com/user-attachments/assets/187b8d0e-1e44-4dbb-bd6b-251c8d770b3c)

### 4. Gene Expression: Female vs. Male Controls

We also compared female and male samples from the non-failing group.

![Female vs Male Control Volcano Plot](https://github.com/user-attachments/assets/2b3385cd-bf17-4751-ad6c-1435dd842458)

### 5. PC1 Distribution

This graph helped us look more closely at how samples were distributed along the first principal component.

![PC1 Distribution](https://github.com/user-attachments/assets/e27a32a3-c3c7-42a1-961b-8663568651e3)

### 6. KEGG Pathway Analysis

We explored which biological pathways were associated with significant gene-expression differences, particularly pathways connected to inflammation and metabolism.

![KEGG Pathway Analysis](sex_differences_analysis/KEGG_Summary_Barplot.png)

## 🔍 What We Found

A few interesting patterns stood out during our analysis:

- **DCM and non-failing hearts showed differences in gene expression**, although the groups weren't completely separated.
- **Male and female DCM samples showed some gene-expression differences**, suggesting that sex may be one factor worth exploring further.
- **Inflammation and metabolic pathways appeared in our pathway analysis**, which may help explain some of the biological changes associated with DCM.
- **There was still a lot of variation between patients**, reminding us that heart disease is influenced by many factors rather than one single gene.

One thing I found especially interesting was that the patterns weren't always as clear-cut as we initially expected. That made the interpretation part of the project just as important as the analysis itself.

## 💭 What I Learned

This project helped me understand how to work with biological data that isn't always simple or straightforward.

I got more experience working with R, exploring large gene-expression datasets and creating visualizations that helped us interpret the results.

It also taught me that finding a pattern in a graph is only the beginning. Understanding what that pattern actually means, and what we *can't* conclude from it, is just as important.

## ⚠️ A Few Limitations

Our results are exploratory, and there are a few things to keep in mind:

- We used bulk RNA-seq data, so we couldn't identify exactly which cell types were responsible for the observed changes.
- Patient differences, including disease severity and treatment history, may affect gene expression.
- Some groups had different sample sizes.
- The findings would need further validation using additional datasets.

These results help us explore possible biological differences, but they don't establish that sex causes differences in DCM severity or progression.

## 💻 Tools We Used

**R • GEOquery • limma • clusterProfiler • org.Hs.eg.db • UMAP • data.table**

## 👩‍🔬 Our Team

This project was completed at **Virginia Commonwealth University**.

- **Vaishnavi Madagiri** — Bioinformatics
- **Ammar Mohiuddin** — Biology and Bioinformatics
- **Harrish Ganesh** — Biology and Bioinformatics
- **Haneia Nemati** — Bioinformatics

## 🌐 Explore the Full Project

Want to see more of the analysis, visualizations and findings?

### [✨ Visit My RNA-seq Project Website](https://vmadagiri.github.io/CardioSeq/)
