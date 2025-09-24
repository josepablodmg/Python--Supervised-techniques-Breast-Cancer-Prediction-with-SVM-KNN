# Breast Cancer Prediction with SVM & KNN

## Project Overview
This project applies supervised machine learning techniques to predict breast cancer tumors as benign or malignant. We use **Support Vector Machines (SVM)** and **K-Nearest Neighbors (KNN)** to classify tumors based on key cellular features. The project also compares model performance and identifies the most influential features.

## Team Members
- José Pablo Del Moral  
- Pol Tordera  
- Ferran Serramalera  
- Bruno Pin  
- Oscar Grau  

## Dataset
The dataset contains measurements of cell nuclei from breast cancer biopsies, including features like radius, texture, perimeter, area, smoothness, compactness, concavity, symmetry, and fractal dimension.  
- Total entries: 569  
- Target: `diagnosis` (0 = benign, 1 = malignant)  

## Methodology
1. **Data Cleaning & Preprocessing**: Removed irrelevant columns and encoded target labels.  
2. **Exploratory Data Analysis (EDA)**: Visualized distributions and correlations, identified top predictive features.  
3. **Modeling**:
   - **SVM**: GridSearchCV to tune hyperparameters; achieved ~95.6% accuracy.  
   - **KNN**: GridSearchCV to optimize neighbors and distance metrics; achieved ~96.5% accuracy.  
4. **Evaluation**: Accuracy, precision, recall, f1-score, and confusion matrices used to compare models.  

## Key Findings
- Most important features: `concave points_worst`, `perimeter_worst`, `concave points_mean`.  
- KNN slightly outperformed SVM in minimizing false negatives, making it preferable for this medical dataset.  
- Features like symmetry and texture had minimal impact on predictions.  

## Conclusion
Both SVM and KNN provide high-accuracy predictions, but KNN is more effective for reducing false negatives. This demonstrates the practical use of supervised techniques in medical diagnostics.

## How to Run
1. Clone this repository.  
2. Load `data.csv` into the Jupyter Notebook `Breast_Cancer_Supervised.ipynb`.  
3. Execute all cells to replicate preprocessing, modeling, and evaluation.  

## License
This project is for educational purposes.
