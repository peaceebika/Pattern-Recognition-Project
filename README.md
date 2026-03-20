# Feature-Based Drought Classification using Pattern Recognition

## Project Overview
This project focuses on the classification of drought and non-drought conditions using satellite imagery. The approach leverages classical computer vision techniques and machine learning models to extract meaningful features and perform classification.

The goal is to support equitable water allocation by enabling accurate identification of drought-affected regions.

---

## Dataset
- Source: Google Earth Engine  
- Total Images: 200  
  - 100 drought images  
  - 100 non-drought images  
- Image Size: 128 × 128 pixels  

---

## Methodology

### 1. Data Preprocessing
- Image resizing (128×128)
- Normalization of pixel values to [0, 1]

### 2. Feature Extraction
- Color Statistics  
  - Mean and standard deviation of RGB channels  

- Color Histograms  
  - 16 bins per RGB channel  

- Texture Features (GLCM)  
  - Contrast  
  - Homogeneity  
  - Energy  

### 3. Model Training
Two machine learning models were implemented:
- Linear Support Vector Machine (SVM)
- Radial Basis Function (RBF) SVM

### 4. Model Evaluation
- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  

---

## Results
- The RBF SVM performed better than the Linear SVM.
- The model showed improved classification for non-linear patterns.
- Some misclassifications still exist.

---

## Key Insights
- Feature-based methods are effective for image classification.
- Color and texture features are important for drought detection.
- Non-linear models (RBF SVM) perform better.

---

## Future Work
- Hyperparameter tuning  
- More advanced feature extraction  
- Larger dataset  
- Real-time satellite integration  

---

## Technologies Used
- Python  
- NumPy  
- OpenCV  
- Scikit-learn  
- Matplotlib  

---

## Project Structure
```
Feature-Based Drought Classification for Equitable Water Allocation Using Pattern Recognition
│
├── README.md
│
├── data
│   ├──drought
│   ├── nondrought
│
├── code
│   └── pattern Recognition.ipynb
│
```

---

## Repository Link
https://github.com/peaceebika/Pattern-Recognition-Project

---

## References
- Bishop, C. M. (2006). Pattern Recognition and Machine Learning  
- Cortes, C., & Vapnik, V. (1995). Support-vector networks  
- Gonzalez, R. C., & Woods, R. E. (2002). Digital Image Processing  
- Haralick, R. M. (1973). Textural features for image classification  

---

## Author
Peace Chinemere Ebika

---

## Note
This project represents the first phase (initial progress) of a larger research objective.
