# Anime Recommendation System

This project implements an **Anime Recommendation System** using machine learning techniques. It classifies anime into various genres based on features such as themes, demographics, popularity, and user-defined inputs to recommend anime titles.

## Table of Contents
- [Dataset](#dataset)
- [Requirements](#requirements)
- [Workflow](#workflow)
- [Models](#models)
- [Results](#results)
- [Visualization](#visualization)
- [How to Run](#how-to-run)

## Dataset
The dataset contains details about various anime titles, including their genres, themes, demographic targets, popularity, and scores. Data preprocessing steps address missing values, scaling, and encoding.

- **Source**: Anime dataset (location based on `/content/drive/MyDrive/Dataset/anime.csv`).

## Requirements
The following libraries are required to run the project:
- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

## Workflow
1. **Data Loading**:
   - Import data from a CSV file stored in Google Drive.
2. **Data Cleaning and Preprocessing**:
   - Handle missing values using median imputation.
   - Encode categorical variables (e.g., themes, demographics).
   - Scale numerical features (e.g., popularity, favorites).
3. **Feature Engineering**:
   - One-hot encode genres for multi-label classification.
   - Add scaled numerical features for model input.
4. **Model Training and Evaluation**:
   - Classifiers: KNN, Decision Tree, and SVM.
   - Evaluate models using accuracy and F1-score.
5. **Recommendation System**:
   - Filter anime based on user input for genres, themes, and demographics.
   - Recommend the top 10 titles sorted by their scores.

## Models
The project implements the following machine learning models:
- **K-Nearest Neighbors (KNN)**
- **Decision Tree Classifier**
- **Support Vector Machine (SVM)**

## Results
- **Performance Metrics**:
  - KNN: Average F1-score of ~0.79.
  - Decision Tree: Average F1-score of ~0.76.
  - SVM: Average F1-score of ~0.80.
- **Insights**:
  - SVM outperforms other models in accuracy and F1-score for most genres.

## Visualization
Key visualizations include:
- Correlation heatmaps of features.
- Genre distribution across the dataset.
- Boxplots and bar charts comparing model performance across genres.

## How to Run
1. Clone the repository or download the notebook file.
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
