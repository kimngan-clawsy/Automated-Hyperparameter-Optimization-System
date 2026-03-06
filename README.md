The dataset can be found at the following: https://drive.google.com/file/d/1LFPs_F9nyHhal5GWxk0qlfizxBOE3xwI/view?usp=drive_link

🧬 Genomics Classification with Hybrid GA-CNN Optimization

📌 Project Overview

This project implements an Automated Machine Learning (AutoML) Pipeline for classifying high-dimensional Genomics data (AML/ALL). The architecture leverages a hybrid approach: CatBoost with SHAP for intelligent feature selection and a Genetic Algorithm (GA) for evolving the optimal hyperparameters of a CNN Ensemble model.

🚀 Key Engineering HighlightsHybrid Feature Selection: 

Utilized CatBoost and SHAP values to reduce dimensionality from 22,277 features to the 50 most significant biomarkers in just ~24 seconds.

Heuristic Optimization: Implemented a custom Genetic Algorithm to automate hyperparameter tuning (Learning Rate, Batch Size, Epoch), ensuring model convergence and superior performance.

Robust Data Integrity: Enforced a strict Hold-out Raw Data splitting strategy to prevent data leakage and provide an unbiased evaluation of model generalizability.

Automated QA & Benchmarking: Built a structured evaluation suite to measure critical production metrics, including Inference Latency and Throughput.


📊 Experimental Results

The following metrics were captured during the final benchmark execution on unseen raw data:

F1-Score (Macro): 99.55%

Accuracy: 99.59%

Inference Latency: 183.10 ms/sample

Throughput: 5.46 samples/sec

Confusion Matrix Insights: The model demonstrates near-perfect classification across AML and ALL subtypes, confirming the effectiveness of the selected genomic biomarkers.


🛠️ Technical Stack

Data Processing: NumPy, Pandas, Scikit-learn.

Machine Learning: CatBoost (Gradient Boosting).

Deep Learning: TensorFlow/Keras (CNN Ensemble).

Explainable AI (XAI): SHAP (SHapley Additive exPlanations).

Optimization: Genetic Algorithm (Evolutionary Computing).

Performance Testing: Automated Benchmarking Suite.  


⚙️ Installation & Usage

Clone the repository

Install dependencies

Hardware Note: GPU acceleration is highly recommended for CatBoost and CNN training.

Execute the pipeline: Open Automated_GA_System.ipynb and run all cells.
