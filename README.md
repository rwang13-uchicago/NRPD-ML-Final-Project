# NRPD-ML-Final-Project README

## Overview
This repository, by Franklin Wang, contains the final coding-based project for DIGS 30009 (Machine Learning for the Humanities). The project analyzes a sampled version of the 2018 **National Repository of Policing Data (NRPD) event data** from Chicago using class-learned machine learning methods.

The goal is not to optimize predictive accuracy, but to evaluate how different models behave when applied to real administrative policing data and to examine the limits imposed by data quality and recording practices.

## Methods
The analysis includes both unsupervised and supervised learning approaches:

### Unsupervised Learning
- K-Means Clustering

### Supervised Learning
- Linear Regression  
- Random Forest Regression  
- Decision Tree Regression  

## Project Workflow
1. Load and inspect the NRPD 2018 events dataset  
2. Clean and preprocess timestamps and categorical variables  
3. Calculate incident delay from dispatch and arrival times  
4. Create exploratory visualizations by radio zone and event type  
5. Apply K-Means clustering to examine data structure  
6. Train supervised models using train/validation/test splits  
7. Evaluate models using R² and MSE  
8. Interpret results and discuss limitations  

## Key Findings
- All supervised models show low explanatory power for incident delay. 
- More flexible models do not outperform linear regression.
- Weak performance reflects data limitations rather than model choice. 
- Categorical recording practices reduce predictive usefulness.  

## Files
- `NRPD_events_2018.csv` – Sampled NRPD events dataset (uploaded via email due to file size)  
- `final_project_notebook.ipynb` – Main analysis Jupyter notebook  
- `README.md` – Project documentation  

## Notes
This final project is only exploratory. Results should not be interpreted as evidence of reliable prediction for predictive policing, but as a solid demonstration of how data quality shapes what machine learning models can learn.
