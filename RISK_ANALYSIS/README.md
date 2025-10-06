**Overview**
This repository demonstrates an **end-to-end risk analytics workflow** for **consumer lending**.  
It covers **credit approval, fraud prevention, model evaluation, monitoring, and dashboard visualization**.  
All datasets are **synthetic or anonymized** to comply with privacy regulations.

Project Structure
- **data/**: Sample datasets (transactions, user login, sales, store info, economics, credit card default data, IV/Correlation, Vintage)  
- **notebooks/**: Jupyter notebooks for the full risk modeling pipeline  
  - 01_data_preprocessing.ipynb  
  - 02_credit_approval.ipynb  
  - 03_fraud_prevention.ipynb  
  - 04_feature_selection.ipynb  
  - 05_model_evaluation.ipynb  
  - 06_monitoring_swap_in_out.ipynb  
  - 07_vintage_analysis.ipynb  
- **dashboards/**: Tableau packaged workbook (`L27_dashboard.twbx`) with interactive visualizations  
- **results/**: Output figures (ROC, KS, Vintage curves)  
- **scorecard.py**: Script to convert logistic regression output into a credit scorecard  
- **requirements.txt**: Python dependencies  

Methodology
1. **Data Preprocessing**  
   - Cleaning, missing value handling, outlier detection  
   - Feature engineering (binning, WOE, IV)  

2. **Credit Approval Model**  
   - Logistic regression baseline  
   - Cut-off score and approval strategy  

3. **Fraud Prevention**  
   - Login anomaly detection  
   - Transaction risk scoring  

4. **Model Evaluation**  
   - ROC, AUC, KS statistics  
   - Confusion matrix, precision-recall  

5. **Monitoring & Vintage**  
   - Stability Index (PSI)  
   - Swap-in/out analysis  
   - Vintage cohort tracking  

6. **Dashboard Visualization**  
   - Approval vs default rate  
   - ROC & KS curves  
   - Fraud distribution  
   - Vintage trends

Results
- **Credit Approval Scorecard**: AUC = 0.75, KS = 0.42  
- **Fraud Model**: Recall = 0.80 on validation set  
- **Monitoring**: Detected feature drift on new 2024 data  
- **Tableau Dashboard**: Interactive view of key metrics

How to Run
```bash
# Clone repository
git clone https://github.com/YourUsername/risk_portfolio.git](https://github.com/Shenghao-Zhang07/first-repo.git
cd RISK_ANALYSIS

Notes on Data and Confidentiality  
To comply with data security and confidentiality policies, all datasets used in this portfolio have been replaced with secure, anonymized, and publicly available data.  
The workflow and analytical results represent the same structure and methodology used in the original risk modeling project, without exposing any internal or client-specific information.  
This portfolio is designed to showcase professional experience in credit risk modeling and data analytics while maintaining full compliance with information protection standards.
