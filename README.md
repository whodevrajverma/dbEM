# dbEM: Database of Epigenetic Modifiers

Welcome to the official documentation overview for **dbEM**, a specialized database developed to maintain and analyze genomic information for epigenetic proteins that serve as potential cancer targets.
This resource compiles extensive data on mutations, expression levels, and gene essentiality to aid in the discovery of epigenetic protein-based cancer therapeutics.

**Database URL:** https://webs.iiitd.edu.in/raghava/dbem/index.php


## Citation

Singh Nanda, J., Kumar, R., & Raghava, G. P. S. (2016).
**dbEM: A database of epigenetic modifiers curated from cancerous and normal genomes.**
*Scientific Reports*, 6, 19340. 
[https://doi.org/10.1038/srep19340](https://doi.org/10.1038/srep19340)

This dataset can also be found on Zenodo at https://doi.org/10.5281/zenodo.20062797

## About the Database

Epigenetics is the study of heritable changes in cellular phenotype that do not involve alterations to the underlying DNA sequence.
Abnormal expression or genomic alterations in chromatin regulators are known to drive oncogenesis. dbEM provides a centralized platform to
analyze the epigenetic landscape in cancer, identifying potential targets for drug development.

The database integrates information from several primary resources:
* **Genomic Variations:** Data retrieved from **COSMIC**, **CCLE**, and the **1000 Genomes Project**.
* **Gene Essentiality:** Sourced from the **COLT-cancer database**.
* **Post-Translational Modifications (PTM):** Compiled from **dbPTM**.

## Key Features

### 1. Comprehensive Protein Catalog
dbEM maintains data for **167 epigenetic proteins**. These are functionally classified into groups such as:
* Histone methyltransferases (HMTs) 
* Chromatin remodelers 
* Histone demethylases (HDMs) 
* DNA methyltransferases (DNMTs) 
* Histone deacetylases (HDACs) and acetyltransferases (HATs) 

### 2. Genomic and Functional Data
* **Mutation Data:** Over 17,000 mutations are filtered and categorized, with **substitution** being the most prevalent type.
* **Expression & CNV:** Includes gene expression and copy number variation data visualized through Circos plots.
* **Gene Essentiality:** Provides GARP scores to highlight which epigenetic proteins are critical for the survival of specific cancer cell lines.

### 3. Structural Information
* **3D Models:** tertiary structures for all 167 proteins modeled using HH suite and Modeller.
* **Domain Mapping:** 837 Pfam and 371 Superfamily domains mapped across the dataset.


### 4. Therapeutic Insights
* **Inhibitor Data:** Information on **54 drug molecules** and small molecule inhibitors.
* **Target Identification:** Analysis highlights highly mutated proteins like **DNMT3A**, **HDAC2**, **KDM6A**, and **TET2** as primary research interests.


## Integrated Web Tools

dbEM includes several user-friendly tools for data analysis:
* **Search Tools:** Simple keyword search, composite search (using logical operators), and similarity-based search.
* **Alignment:** Visualize sequence conservation and evolutionary trees via Jalview and ClustalW.
* **Profile-Based Prediction:** Predicts if a protein change is a normal variation (SNP) or a cancer-causing mutation based on HMM profiles.
* **HMM/PSSM Profiles:** Conservation scores generated for each protein.


## Technical Architecture

The database is built on a standard technology stack for reliability and performance:
* **Backend:** MySQL server for data storage and retrieval.
* **Web Server:** Apache HTTP Server.
* **Frontend:** Developed using PHP, HTML, CSS, and Java, with PERL scripts for the interface.

## Contact & Acknowledgements

The project was conceived and coordinated by **Gajendra Raghava**. Financial support was provided by the **Council of Scientific and Industrial Research (CSIR)**,
the **University Grant Commission (UGC)**, and the **Department of Biotechnology (DBT)**, Govt. of India.

**Correspondence:** raghava@iiitd.ac.in
