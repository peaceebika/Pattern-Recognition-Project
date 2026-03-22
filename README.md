---
title: "Feature-Based Drought Classification for Equitable Water Allocation: A Pattern Recognition Approach"
name: "Peace Chinemere Ebika"
course: Pattern Recognition
---
# Feature-Based Drought Classification for Equitable Water Allocation: A Pattern Recognition Approach

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
- The Linear SVM and RBF SVM models produced comparable performance.
- The models showed limited ability to clearly separate drought and non-drought classes.
- Some misclassifications still exist, indicating the need for improvement.

---

## Key Insights
- Feature-based methods are effective for image classification.
- Color and texture features are important for drought detection.
- Current models show similar performance, suggesting the need for improved feature representation.

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
Feature-Based Drought Classification for Equitable Water Allocation: A Pattern Recognition Approach
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

## Google Earth Engine
The Google Earth Engine script used to filter, visualize, and export the satellite imagery can be accessed here:

[View the Earth Engine Code](https://code.earthengine.google.com/ed452eed789f12fa058f102ea639b09e?noload=1)

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
