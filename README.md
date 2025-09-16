# Lightweight Machine Learning Methodology for Wirelength Prediction Using Pre-Routing Features

This repository contains the implementation of a **lightweight machine learning framework** for **early wirelength prediction** in VLSI design.  
The methodology leverages **pre-routing design features** extracted from DEF/LEF files and applies **classical regression models** and **ensemble techniques** to estimate global wirelength prior to detailed routing.  

---

## 🚀 Key Features
- **DEF/LEF Parser**: Extracts design-level features such as DieWidth, DieHeight, NumInstances, NumValidPins, NumNets, etc.  
- **Feature Ablation Analysis**: Identifies the most influential features for accurate prediction.  
- **Model Training**: Implements regression models (KNeighbors, XGBoost, RandomForest, and Ensembles).  
- **Lightweight Deployment**: Focus on small model size, low inference time, and minimal RAM usage.  
- **Benchmarking**: Evaluated on **ISPD 2018, ISPD 2019, and CircuitNet N28** datasets.  

---

## 📊 Experimental Results
- **Top Features Identified**: DieWidth, NumInstances, NumValidPins, DieHeight.  
- **Best Models**: KNeighbors, XGBoost, RandomForest.  
- **Ensemble Strategy**: Voting Ensemble combining the above models improved robustness.  
- **Performance**: Achieved up to **R² = 0.95** with compact models suitable for low-resource deployment.  

For detailed results, see [`experiments/`](./experiments).  
<img width="1447" height="717" alt="flow" src="https://github.com/user-attachments/assets/65d5f4e0-0334-4187-8355-4d2d64cac395" />

---

## 📂 Repository Structure

