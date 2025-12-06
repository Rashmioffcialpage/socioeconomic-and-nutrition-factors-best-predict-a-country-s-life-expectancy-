📊 Clustering Countries Using Socio-Economic & Health Indicators
✨ Overview

This project applies unsupervised statistical learning techniques to cluster 167 countries based on key health, economic, and demographic indicators. The goal is to support data-driven decisions for international aid allocation by identifying patterns among countries with similar development challenges.

Using PCA for dimensionality reduction and K-Means for clustering, the project uncovers four distinct clusters that highlight differences in life expectancy, child mortality, GDP, health expenditure, and population size.

🚀 Key Features

🔍 Exploratory Data Analysis (EDA)
Histograms, heatmaps, distribution checks, correlation patterns.

🧮 Inferential Statistics
Two-sample t-test comparing under-5 mortality in high-GDP vs low-GDP countries.
Result: p < 0.001, large effect size.

🧠 Unsupervised Learning Methods

🧊 Principal Component Analysis (PCA) → Reduced 5 features to 2 components while retaining 78% variance.

🎯 K-Means Clustering (K=4) → Identified four distinct country groups.

🤖 Supervised Learning (Extended Model Exploration)

🌲 Random Forest Regressor → R² = 0.9943, RMSE = 0.74

⚡️ XGBoost Regressor for performance verification

💡 Feature importance shows birth rate and death rate are top predictors of life expectancy.

📌 Ethical Considerations
Bias risks, uneven data representation, impact on aid allocation decisions.

🗂 Dataset

📁 country_data.csv

🌐 Source: Kaggle – Unsupervised Learning on Country Data

✔️ 167 countries

✔️ No missing values

✔️ Features include:

Life Expectancy

GDP per Capita

Under-5 Mortality

Government Health Expenditure

Total Population

🛠 Methodology

Preprocessing

Standardization via StandardScaler

Dimensionality Reduction

PCA to handle multicollinearity

Clustering

K-Means (random_state=42)

Elbow method used to determine optimal K

Model Evaluation

Cluster visualization

Feature contribution interpretation

Supervised Model Validation

Random Forest & XGBoost predictions

Feature importance ranking

📈 Results
🔹 PCA Findings

PC1 (62%): Economic + health indicators

PC2 (16%): Population/demographics

🔹 Cluster Highlights

Cluster 0 → Low life expectancy, high child mortality → Highest aid priority

Cluster 1 → High-income, strong health outcomes

Cluster 2 & 3 → Mixed development profiles

🔹 Key Insights

Birth rate (42%) and death rate (16%) are the strongest drivers of life expectancy

GDP has surprisingly lower predictive power

Random Forest delivers near-perfect predictions

🧭 Discussion

🏁 Clusters match known global development patterns

⚠️ Bias concerns — Africa dominates the lowest-development cluster

🕒 Dataset is cross-sectional, limiting temporal insights

🔄 K selection affects cluster interpretation

🎯 Recommendations

Prioritize Cluster 0 for health infrastructure aid

Add time-series indicators for future modeling

Use hierarchical clustering to validate K-Means

Update dataset with latest global development stats

Explore supervised models for cluster prediction

📚 References

Include:

Kaggle dataset (Rohan Rao)

World Bank indicators

UNDP development reports

PCA & clustering academic references

🙌 Authors

👩‍💻 Rashmi Thimmaraju
📧 rashmi.lnu@my.liu.edu

