# Predicting Favorable Outcomes for MedCamp Events

## Overview
This repository contains the analysis, feature engineering, and modeling steps to predict favorable outcomes for MedCamp events. The goal is to optimize inventory and improve participant experience by understanding key factors that influence event outcomes.

---

## Problem Statement
MedCamp, a not-for-profit organization, faces challenges with high drop-offs between registrations and actual participation in their health camps. The project aims to:
- Predict the probability of favorable outcomes for each participant.
- Use predictions to optimize resource allocation and improve the participant experience.

---

## Data Description
The dataset consists of:
1. **Health Camp Details:** Information about camp dates and types.
2. **Patient Profiles:** Demographics and social media activity of participants.
3. **Registration Data:** Records of patient registrations for various health camps.
4. **Attendance Data:** Details of patient attendance and engagement at health camps.

All datasets are stored in the `data/` directory.

---

## Key Steps
1. **Data Preprocessing:**
   - Handling missing data.
   - Merging multiple datasets for unified analysis.

2. **Feature Engineering:**
   - Creating derived features like `Interaction_Days` and `Waiting_Period`.
   - Encoding categorical variables.
   - Aggregating patient and health camp metrics.

3. **Model Building:**
   - Baseline models: Decision Tree, Random Forest, Gradient Boosting.
   - Advanced models: XGBoost, LightGBM.
   - Ensemble models: Stacking classifier with LGBM as the meta-model.

4. **Evaluation:**
   - Metrics: AUC-ROC, Precision-Recall, Log Loss.

---

## Results
- **Best Model:** Gradient Boosting (AUC-ROC: 0.75)
- **Submission File:** Stored in the `outputs/submission/` directory.

---

## Project Structure
