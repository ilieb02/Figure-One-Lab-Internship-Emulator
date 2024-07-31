# F1L Internship Emulator

(in progress)

## Introduction

This repository is dedicated to documenting my progress in the Figure One Lab Intership Emulator by Dean Lee, as introduced in his [LinkedIn Newsletter](https://www.linkedin.com/pulse/introducing-f1l-internship-emulator-dean-lee-xckee/). 

The purpose of this project is to emulate the work a computational biology intern in biotech/pharma would do over the course of six weeks.

## The Key Scientific Question (KSQ)

The key scientific question for this project is the following:

How can we explore available single cell RNA-seq data from cancer cell lines to explore the use of the FDA-approved drugs Trastuzumab and Bevacizumab in other cancers?

### Additional questions

We can derive additional questions for further analysis:

Can we infer sensitivity to Trastuzumab oder Bevacizumab in other cancers from the available scRNA-seq data from cancer cell lines?

Can we identify additional cancer cell lines with heightened expression of HER2 or VEGF?

### Concept Review

- **Trastuzumab**: Targets HER2 and is used in the treatment of HER2-positive breast and gastric cancers.
    - recombinant monoclonal IgG1 antibody that targets human epidermal growth factor receptor 2 (HER2)
    - targets extracellular domain of HER2 by blocking its cleavage as well as HER2 dimerization, thereby inhibiting tyrosine kinase activity
    - also mediates activation of antibody-dependent cell-mediated cytotoxicity (ADCC) and subsequent cell lysis as well as endocytosis of HER2
    - indicated for HER2 overexpression or HER2 gene amplification
- **Bevacizumab**: Targets VEGF and is used for a variety of cancers, including colorectal, lung, glioblastoma, breast, liver, and kidney cancer.
    - binds to vascular endothelial growth factor (VEGF), thereby inhibiting binding to VEGFR and inhibiting angiogenesis

### Cancer cell lines

Cancer cell lines are used as models for studying cancer biology, validating drug targets and evaluating drug efficacy.

Cancer cell lines correlate in chromosomal copy number, gene expression patterns and point mutation frequency with primary tumors (Barretina et al. 2012), and therefore may be used as representatives of primary tumors.

However, cancer cell lines are genomically instable and passaging of cell lines results in genetic and transcriptional heterogeneity which in turn leads to variability in cell morphology, doubling time,  or drug sensitivity. This genetic variation affects reproducibility of experiments (Ben-David et al. 2018), and therefore variation across strains has to be taken into account for experimental design and data analysis.

### Single Cell RNA-sequencing

Single cell RNA-sequencing (scRNA-seq) allows for gene expression analysis at single cell level, capturing cellular heterogeneity within tissues.

Multiomics approaches can couple scRNA-seq with single cell surface proteome or CRISPR perturbation screens.

## The Paper

The aim of this project is to explore the data from Kinker et al. (2020) and to re-create Figure 1 (and possibly other figures) from the paper.

### Questions for deeper understanding

**How did the authors handle the potential caveat of co-culturing cell lines before profiling by scRNA-seq? Why do you think that caveat was or was not adequately addressed?**

**The authors identified discrete subpopulations of cells within a subset of individual cell lines (Fig. 2A-B). What might be the reason why some cell lines have these discrete subpopulations while others do not?**

**What are Recurrent Heterogeneous Programs (RHPs) and how were they defined?**

**How do the identified RHPs relate to in vivo programs of heterogeneity in tumors, and what evidence supports this relationship?**

**Where can you download the scRNA-seq data as shown in Figure 1B?**

Data can be downloaded from the Broad Institute’s Single Cell Portal under the reference SCP542

### References

Barretina, J., Caponigro, G., Stransky, N. *et al.* The Cancer Cell Line Encyclopedia enables predictive modelling of anticancer drug sensitivity. *Nature* **483**, 603–607 (2012). https://doi.org/10.1038/nature11003

Ben-David, U., Siranosian, B., Ha, G. *et al.* Genetic and transcriptional evolution alters cancer cell line drug response. *Nature* **560**, 325–330 (2018). https://doi.org/10.1038/s41586-018-0409-3

Kinker, G.S., Greenwald, A.C., Tal, R. et al. Pan-cancer single-cell RNA-seq identifies recurring programs of cellular heterogeneity. Nat Genet 52, 1208–1218 (2020). https://doi.org/10.1038/s41588-020-00726-6