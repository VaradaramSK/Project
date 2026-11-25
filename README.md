# Beyond Accuracy: Imputation's Real Impact on Downstream Prediction

## Description

A research-based platform for evaluating missing-data imputation techniques and analyzing their impact on downstream machine learning prediction performance using the MEPS dataset. The system compares multiple imputation methods under different missing-data rates and missingness mechanisms to determine whether better imputation accuracy leads to better predictive outcomes.

## About

**Beyond Accuracy: Imputation's Real Impact on Downstream Prediction** is a project designed to investigate the real-world impact of missing-data imputation techniques on machine learning prediction tasks. Traditional imputation evaluation focuses primarily on how accurately missing values are reconstructed. However, an imputation method with lower reconstruction error does not necessarily produce better downstream prediction results.

This project addresses this problem by evaluating five imputation methods—Mean, K-Nearest Neighbors (KNN), Regression, Multiple Imputation by Chained Equations (MICE), and Random Forest—under different missing-data rates and missingness mechanisms, including MCAR and MNAR.

Using a fixed MEPS dataset, the system artificially introduces missing values, applies selected imputation techniques, evaluates imputation quality using RMSE and MAE, and measures downstream prediction performance using metrics such as AUC. The results are presented through an interactive dashboard, allowing researchers to compare methods and understand how missingness affects prediction performance.

## Features

- Uses a fixed MEPS dataset for consistent and reproducible experiments.
- Supports multiple missing-data rates: 5%, 15%, 30%, 50%, 60%, and 70%.
- Simulates different missingness mechanisms, including MCAR and MNAR.
- Implements five imputation techniques:
  - Mean Imputation
  - K-Nearest Neighbors (KNN)
  - Regression Imputation
  - Multiple Imputation by Chained Equations (MICE)
  - Random Forest Imputation
- Evaluates imputation quality using RMSE and MAE.
- Evaluates downstream prediction performance using AUC.
- Compares imputation methods across different missingness conditions.
- Provides interactive visualizations and result dashboards.
- Tracks experiment progress and status.
- Allows researchers to export imputed datasets and experiment results.
- Supports reproducible experimentation and method comparison.

## Requirements

- **Operating System:** Windows 10/11 or Linux (64-bit).
- **Programming Language:** Python 3.8 or later for machine learning and data processing.
- **Frontend Development:** React.js with Vite.
- **Backend Development:** Node.js and Express.js.
- **Database:** MongoDB for storing users, experiment configurations, results, and reports.
- **Machine Learning Frameworks:** Scikit-learn for imputation and prediction models.
- **Data Processing Libraries:** Pandas and NumPy for dataset processing and numerical computation.
- **Statistical Libraries:** SciPy and Statsmodels for statistical operations where required.
- **Visualization:** Recharts for interactive charts and result visualization.
- **API Development:** FastAPI for communication with the Python machine-learning service.
- **Authentication:** JWT and bcryptjs for secure user authentication.
- **Version Control:** Git and GitHub for source-code management.
- **IDE:** Visual Studio Code for development, debugging, and project management.

## System Architecture

The system consists of three main components:

1. **Frontend:** React.js application for dataset viewing, experiment configuration, progress monitoring, and result visualization.
2. **Backend:** Node.js and Express.js API for authentication, experiment management, database operations, and communication with the machine-learning service.
3. **Machine Learning Service:** Python-based FastAPI service that performs data preprocessing, missingness generation, imputation, evaluation, and downstream prediction.

### Workflow

Researcher  
↓  
React Frontend  
↓  
Node.js / Express Backend  
↓  
FastAPI Machine Learning Service  
↓  
Fixed MEPS Dataset  
↓  
Missingness Simulation  
↓  
Imputation Methods  
↓  
Imputation Evaluation (RMSE / MAE)  
↓  
Downstream Prediction  
↓  
Prediction Evaluation (AUC)  
↓  
Results Stored in MongoDB  
↓  
Interactive Results Dashboard

## Output

### Output 1 – Missingness Configuration

The researcher selects the missing-data rate, missingness mechanism, imputation methods, and prediction task before running the experiment.

### Output 2 – Experiment Progress

The system displays the current experiment status, progress percentage, and processing stage while the experiment is running.

### Output 3 – Imputation Performance Comparison

The system compares the imputation techniques based on RMSE and MAE across different missing-data rates and missingness mechanisms.

### Output 4 – Downstream Prediction Performance

The system visualizes prediction performance using AUC and allows comparison of the downstream impact of different imputation techniques.

### Output 5 – Results Dashboard

The results dashboard provides a comprehensive comparison of the selected methods using tables, charts, and experiment summaries.

*Actual screenshots and measured results should be added after implementation and evaluation.*

## Results and Impact

The project aims to demonstrate that imputation quality should not be evaluated solely based on reconstruction accuracy. By comparing RMSE and MAE with downstream prediction performance, the system investigates whether the imputation method that reconstructs missing values most accurately also produces the best predictive results.

The experiments help identify how imputation performance changes under increasing missing-data rates and different missingness mechanisms, particularly MCAR and MNAR.

The platform provides researchers with a systematic framework for:

- Comparing different imputation techniques.
- Understanding the effects of missing-data rates on prediction performance.
- Investigating differences between MCAR and MNAR conditions.
- Identifying imputation methods that perform well for downstream prediction.
- Evaluating the relationship between imputation accuracy and predictive effectiveness.

The project contributes to a more practical evaluation of missing-data handling in machine learning by emphasizing the impact of imputation on the final prediction task rather than focusing only on reconstruction accuracy.

## Articles Published / References

Add the research papers, datasets, and articles that were actually used during the development of this project.

Suggested reference categories:

1. Research papers on missing-data mechanisms (MCAR, MAR, and MNAR).
2. Research papers on Mean, KNN, Regression, MICE, and Random Forest imputation.
3. Research papers examining the relationship between imputation quality and downstream machine-learning prediction performance.
4. Documentation and research resources related to the Medical Expenditure Panel Survey (MEPS).
5. Scikit-learn documentation for preprocessing, imputation, and machine-learning evaluation.

