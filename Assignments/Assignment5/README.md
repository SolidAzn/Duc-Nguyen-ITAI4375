# Assignment 5 — Machine Learning Prognostic Model Analysis: SFTS Mortality Prediction

**Course:** ITAI 4375 — AI in Healthcare  
**Date:** February 16, 2026  

---

## Problem

Severe Fever with Thrombocytopenia Syndrome (SFTS) is a tick-borne viral disease with mortality rates approaching 30%. Clinicians managing SFTS patients in emergency settings need reliable, early risk stratification tools to identify which patients are most likely to deteriorate. This assignment analyzed a published study (Xu et al., 2025) that developed an XGBoost machine learning model to predict SFTS mortality.

## Approach

I performed a structured critical analysis of the study, examining:

- The **feature selection**: 7 clinical variables collected at hospital admission (consciousness level, AST, urea, CRRT requirement, LDH, lymphocyte count, mechanical ventilation status)
- The **model architecture**: XGBoost algorithm with SHAP (SHapley Additive exPlanations) for interpretability
- The **validation strategy**: Internal validation (AUC = 0.911) and external validation on an independent cohort (AUC = 0.891)
- The **clinical deployment tool**: A web-based Streamlit application for real-time risk assessment

I also critically evaluated the model's strengths and limitations, particularly around generalizability and performance in high-severity patients.

## Results & Key Findings

The model demonstrated excellent predictive performance (AUC > 0.9 is considered highly accurate). Importantly, the integration of SHAP analysis addresses the "black box" problem — clinicians can see exactly which factors drove a given patient's risk score. However, the study population came exclusively from two hospitals in eastern China, raising legitimate questions about how well the model generalizes to other geographic regions, ethnic populations, and healthcare settings.

## What I Learned

This assignment gave me a framework for critically evaluating any published ML model in healthcare — not just accepting impressive AUC numbers at face value, but asking: Who was this model trained on? How was it validated? Where does it fail? These questions matter enormously when the output influences life-or-death clinical decisions.
