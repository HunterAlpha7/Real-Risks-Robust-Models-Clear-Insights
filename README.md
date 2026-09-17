# Real Risks, Robust Models, Clear Insights: Explainable Ensemble Learning for Flood Risk in Bangladesh

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HunterAlpha7/Real-Risks-Robust-Models-Clear-Insights/blob/main/CatBoost%2BRF.ipynb)

This repository contains the code, data analysis, and LaTeX source for the paper **"Real Risks, Robust Models, Clear Insights: Explainable Ensemble Learning for Flood Risk in Bangladesh"**. 

The study introduces a highly accurate, transparent, and explainable machine learning framework to predict flood probabilities using a heterogeneous voting ensemble of **CatBoost** and **Random Forest** algorithms, tailored for the complex hydrological environment of the Bengal Delta.

## 📌 Key Features

- **Advanced Ensemble Modeling**: Combines the gradient boosting efficiency of CatBoost with the variance-reducing bagging of Random Forest for exceptional robustness and prediction stability.
- **Domain-Specific Feature Engineering**: Extracts higher-order risk indicators such as *Infrastructure Vulnerability*, *Environmental Degradation*, and *Monsoon-Drainage Interaction* from 20 environmental and socio-economic factors.
- **Explainable AI (XAI)**: Integrates SHAP (SHapley Additive exPlanations) to demystify the "black box" model, providing clear insights into how individual factors like monsoon intensity or river management contribute to flood risks.
- **High Predictive Power**: Achieves state-of-the-art results on a 50,000-record dataset through 5-fold cross-validation.

## 📊 Performance Metrics

Our CatBoost + Random Forest ensemble model outperforms baseline methods (like XGBoost + RF and LightGBM + RF) with the following regression metrics:

| Metric | Score |
| ------ | ----- |
| **$R^2$ Score** | `0.9719` |
| **RMSE** | `0.0084` |
| **MAE** | `0.0064` |

When converting continuous probability outputs into a discrete binary classification (threshold $\tau = 0.5$):

- **Accuracy**: 95.52%
- **Precision**: 98.74%
- **Recall**: 94.47%
- **F1-Score**: 0.9554

## 📂 Repository Structure

- `CatBoost+RF.ipynb`: A complete Jupyter Notebook containing data preprocessing, feature engineering, model training, evaluation, and SHAP visual interpretations. Designed to run seamlessly in Google Colab.
- `main.tex`: The LaTeX source code of the academic paper detailing the methodology, results, and discussions.
- `LICENSE`: Licensing information for this project.

## 🚀 Getting Started

### Prerequisites

You can run the notebook locally or via Google Colab. If running locally, ensure you have Python 3.8+ installed along with the required libraries.

```bash
pip install pandas numpy scikit-learn catboost shap matplotlib seaborn
```

### Running the Code

1. Clone the repository:
   ```bash
   git clone https://github.com/HunterAlpha7/Real-Risks-Robust-Models-Clear-Insights.git
   cd Real-Risks-Robust-Models-Clear-Insights
   ```
2. Open the `CatBoost+RF.ipynb` notebook in Jupyter or upload it to Google Colab.
3. The dataset used is the [Flood Prediction Dataset](https://www.kaggle.com/datasets/naiyakhalid/flood-prediction-dataset) from Kaggle. Ensure the dataset path is updated correctly in the notebook if running locally.

## 🧠 Core Insights from SHAP Analysis

The SHAP analysis revealed that hydrological factors (e.g., *Environmental Degradation*, *Climate/Natural Hazards*, and *Infrastructure Vulnerability*) are the primary drivers of flood risk, heavily reflecting the reality of Bangladesh's susceptibility to heavy monsoon rains and river overflows. Secondary factors such as *Encroachments*, *Population Score*, and *Urbanization* also play a significant role, emphasizing the importance of infrastructure maintenance and resilient urban planning.

## 📝 Citation

If you use this code or our findings in your research, please refer to the accompanying paper included in this repository.

## 👥 Authors

**Seyam Bin H Rahman**  
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:Seyam_Rahman7@proton.me)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](#)

**Nafia Anjum Khan**  
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:anjumturna170@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/nafia-anjum)

**Namira Hossain**  
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:namiranitu@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](#)

**Omar Saad Majumder Nihal**  
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:saad.nihal77@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/omar-saad-majumder-nihal-30a5a9300)

## 📄 License

This project is licensed under the terms found in the [LICENSE](./LICENSE) file.