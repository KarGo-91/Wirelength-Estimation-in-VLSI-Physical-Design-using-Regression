# Lightweight Machine Learning Methodology for Wirelength Prediction Using Pre-Routing Features

This repository presents a **lightweight machine learning framework** for **early wirelength prediction** in VLSI design.  
The approach leverages **pre-routing features** extracted from DEF/LEF files and applies **classical regression models** with ensemble techniques to estimate global wirelength before detailed routing.  

---

## 🚀 Key Highlights
- **DEF/LEF Parsing** → Extracts essential design features such as *DieWidth, DieHeight, NumInstances, NumValidPins, NumNets*, etc.  
- **Feature Ablation Study** → Identifies the most influential features contributing to wirelength estimation.  
- **Model Training** → Implements lightweight regressors (KNeighbors, XGBoost, RandomForest) and ensemble methods.  
- **Resource-Efficient Deployment** → Prioritizes small model size, low latency, and minimal RAM usage.  
- **Benchmarking** → Validated on **ISPD 2018, ISPD 2019, and CircuitNet-N28** datasets.  

---

## 📊 Experimental Findings
- **Key Predictors**: DieWidth, NumInstances, NumValidPins, and DieHeight emerged as dominant features.  
- **Strong Performers**: KNeighbors, XGBoost, and RandomForest delivered the best results.  
- **Robustness**: An ensemble strategy combining these models further improved accuracy.  
- **Performance**: Achieved up to **R² = 0.95** with compact models suitable for low-resource environments.  

---

## 🖼️ Block Diagram

The overall workflow of the proposed methodology is illustrated below:
<img width="1447" height="717" alt="flow" src="https://github.com/user-attachments/assets/51ff0a42-aa15-452c-9911-41cdf208e4f2" />



**Workflow Description**:  
1. **Inputs** → DEF/LEF files are parsed to obtain *pre-routing features*.  
2. **Feature Extraction** → Collects design-level attributes before routing.  
3. **Modeling** → Trains lightweight ML regressors (KNeighbors, XGBoost, RandomForest) and ensembles.  
4. **Output** → Provides early wirelength estimation in the **Physical Design Flow**, enabling faster design space exploration and optimization.  

---
