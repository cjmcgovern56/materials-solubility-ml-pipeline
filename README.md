# Predictive Materials Property & Solubility Modeling Pipeline (MLR & KNNR)

## 🔗 Portfolio Deep Dive
*This computational architecture forms a core pillar of my engineering portfolio. For the complete interactive data study, manufacturing contexts, and structural applications, visit the [Data Science & ML Pipelines Page on my Website].*

---

## 📊 Project Overview
Evaluating advanced materials property combinations and solubility boundaries through traditional experimental trial-and-error is exceptionally resource-intensive and creates development bottlenecks. 

This repository provides an automated, supervised machine learning pipeline engineered to ingest high-dimensional molecular property descriptors, transform feature spaces via standardized scaling, and accurately forecast continuous physical outcomes (such as fluid-polymer solubility limits). 

## 🛠️ Tech Stack & Dependencies
* **Core Language:** Python
* **Data Scaffolding:** Pandas, NumPy
* **Machine Learning Suite:** Scikit-learn (`LinearRegression`, `KNeighborsRegressor`, `StandardScaler`, `train_test_split`)
* **Visualization Engine:** Seaborn, Matplotlib

## 🚀 Architectural Breakdown

### 1. High-Dimensional Ingestion & Synthesis
The workspace models complex, multi-variable material descriptor domains—including molecular weights, melting points, polar surface areas, and rotatable/hydrogen bond metrics—mapping them out to evaluate non-linear structural signals.

### 2. Feature Scale Normalization
To prevent distance-metric distortions within the K-Nearest Neighbors architecture, features are normalized using a Z-score `StandardScaler`. This configuration guarantees that distinct units (e.g., Temperature vs. Weight) contribute proportionally to model spatial vectors.

### 3. Dual-Architecture Modeling & Validation
The pipeline executes and evaluates two distinct algorithm frameworks side-by-side to establish optimal predictive integrity:
* **Multiple Linear Regression (MLR):** Maps foundational baseline property vectors and calculates directional coefficients.
* **K-Nearest Neighbors Regression (KNNR):** Utilizes distance-weighted neighbor vectors to map localized non-linear clusters.

### 4. Cross-Validation Performance
Model execution achieves a high-impact validation milestone, securing an **$R^2$ score of 0.91 (91% accuracy)**. The script auto-generates a publication-quality `solubility_predicted_vs_actual.png` scatter plot with a 1:1 parity line to visually audit variance trends.

---

## 📁 Repository Map
* `src/solubility_pipeline.py`: Main execution script detailing data splitting, Z-score transformations, multi-model evaluation, and automated plot generation.
* `solubility_predicted_vs_actual.png`: The cross-validation performance visual demonstrating output accuracy against experimental reality.
