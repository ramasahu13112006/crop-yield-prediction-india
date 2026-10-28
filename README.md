# crop-yield-prediction-india
# 🌾 Crop Yield Prediction using Deep Learning 🚀

A robust, end-to-end Machine Learning and Deep Learning project designed to forecast crop yield based on environmental factors, historical rainfall, temperature data, and regional parameters. This repository contains data preprocessing pipelines, deep learning neural network architectures, saved model artifacts, and an interactive web application interface.

---

## 🛠️ Tools & Technologies Used

Below is the complete technology stack used to build, train, evaluate, and deploy this project:

### 🐍 Programming & Environment
- **Python (v3.10+)**: Primary programming language for data engineering, model development, and backend setup.
- **VS Code / Google Colab**: Development environments for model training (GPU acceleration) and repository structuring.

### 🧠 Deep Learning & Machine Learning Frameworks
- **TensorFlow / Keras**: Built the Sequential Deep Neural Network architecture featuring Batch Normalization, Dropout layers, and custom optimizers.
- **Scikit-Learn**: Handled data preprocessing (`StandardScaler`, `OneHotEncoder`), train-test splitting, and baseline model evaluation (`RandomForestRegressor`).

### 📊 Data Manipulation & Analytics
- **Pandas**: Efficient structured data manipulation, feature extraction, and CSV cleaning (`yield_df.csv`).
- **NumPy**: Matrix and high-dimensional array operations for neural network inputs.

### 🎨 Visualizations & Analytics
- **Matplotlib & Seaborn**: Static plots for EDA, feature correlation heatmaps, loss curves, and evaluation error distribution.
- **Chart.js**: Dynamic, interactive charts embedded in the web dashboard UI for yield comparisons.

### 💾 Model Serialization & Storage
- **HDF5 (`.h5`)**: Saved deep neural network weights and architecture (`ultimate_crop_yield_dl_model.h5`).
- **Pickle / Joblib**: Serialized scaler object (`scaler.pkl`) for consistent inference feature scaling.

### 🌐 Frontend & Web Application UI
- **HTML5 & CSS3**: Responsive web layout with Glassmorphism aesthetic and neon accent styling.
- **Tailwind CSS**: Utility-first CSS framework for UI styling, dark mode aesthetics, and dynamic layout rendering.
- **JavaScript (ES6+)**: Interactive client-side logic, real-time input sliders, and asynchronous API calls.

### ⚡ Backend Server & Deployment
- **Flask / FastAPI**: Lightweight Python Web Framework to expose REST API endpoints for model inference.
- **Git & GitHub**: Version control, artifact tracking, and public repository management.

---

## 📌 Project Overview

Accurate crop yield prediction plays a vital role in agricultural planning, risk management, and food security. This project leverages advanced **Deep Learning (Sequential Neural Networks)** with **Batch Normalization** and **Dropout Regularization** to capture complex non-linear relationships in agricultural datasets.

### Key Highlights:
- **Comprehensive Preprocessing:** Handled categorical encoding (One-Hot Encoding for State/Region and Crop Item) and feature scaling using `StandardScaler`.
- **Model Iteration & Evaluation:** Benchmarked a baseline Machine Learning model (Random Forest, $R^2 \approx 0.9876$) before architecting an **Ultimate Deep Learning Model** achieving a **Test MAE of ~7665 hg/ha**.
- **Saved Pipeline Artifacts:** Exported feature scalers and trained neural network models for seamless integration into web services.
- **Interactive Web Interface:** User-friendly UI featuring real-time prediction, environmental factor breakdowns, and agricultural advisories.

---

## 📂 Repository Directory Structure

```text
crop-yield-prediction-india/
│
├── data/
│   ├── raw/
│   │   └── yield_df.csv                    # Raw Kaggle dataset
│   └── processed/
│       └── final_cleaned_yield.csv          # Cleaned & preprocessed dataset
│
├── artifacts/                               # Pre-trained model & transformation weights
│   ├── ultimate_crop_yield_dl_model.h5      # Keras Deep Neural Network trained model
│   └── scaler.pkl                           # StandardScaler object for feature normalization
│
├── notebook/
│   └── crop_yield_dl_training.ipynb        # Colab notebook containing EDA, training & evaluation
│
├── app/                                     # Web application module
│   ├── index.html                           # Glassmorphism interactive web app interface
│   └── app.py                               # Flask / FastAPI backend script
│
├── requirements.txt                         # Python project dependencies
└── README.md                                # Project documentation
