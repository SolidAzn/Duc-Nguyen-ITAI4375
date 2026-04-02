# Assignment 6 — Genetic Testing as Non-Traditional Health Data

**Course:** ITAI 4375 — AI in Healthcare  
**Date:** March 2, 2026  

---

## Problem

Traditional clinical data — lab results, vitals, imaging — tells us about a patient's current health. Genetic data is fundamentally different: it can reveal disease risk before any symptoms appear. This assignment examined genetic testing as a form of non-traditional health data and evaluated its role in precision medicine and preventive care.

## Approach

I analyzed two major forms of genetic testing:

- **Single-gene mutation analysis** (e.g., BRCA1/BRCA2 for hereditary cancer risk)
- **Polygenic risk scoring (PRS)**, which aggregates thousands of small genetic variants to estimate risk for complex diseases like coronary artery disease and type 2 diabetes

I reviewed large-scale genomic studies (including a study of nearly 500,000 adults by Inouye et al., 2022, and research published in the New England Journal of Medicine by Khera et al., 2023) to evaluate real-world evidence for clinical utility. I also addressed the significant ethical and equity challenges surrounding genetic data.

## Results & Key Findings

The evidence supports genetic testing's value in enhancing cardiovascular disease risk prediction beyond traditional clinical markers. However, calibration across diverse ancestral populations remains a critical unsolved problem — many PRS models perform well in European-ancestry populations but less reliably in others, raising serious equity concerns about who benefits from precision medicine.

## What I Learned

Genetic data is powerful, but it is not neutral. How a model is trained determines who it serves well and who it underserves. This assignment deepened my understanding of how AI systems can inadvertently encode and amplify existing health disparities if dataset diversity and equity are not prioritized from the start. Strong governance frameworks are not optional extras — they are prerequisites for responsible deployment.
