#  Stress Detection from ECG Signals

This project aims to detect stress levels using ECG signals through a machine learning pipeline. By analyzing physiological data from the WESAD dataset, the model classifies states such as **stress** and **no stress**, helping explore the potential of wearable health monitoring systems.

---

##  Project Overview

Stress detection is a key application in health informatics and mental well-being. In this project, we build a machine learning pipeline to classify emotional states using ECG signals collected from chest-worn sensors. The ECG data was preprocessed and converted into features based on **Heart Rate Variability (HRV)**, followed by training and evaluation of classification models.

---

##  Features

- Signal preprocessing from raw ECG time-series  
- HRV-based feature extraction  
- Emotion-state classification (e.g., stress vs. no stress)  
- Visualization of ECG signals and feature distributions  
- Model training and evaluation using classification metrics

---

##  Technologies Used

- Python  
- NumPy, Pandas  
- Scikit-learn  
- Matplotlib, Seaborn  
- WESAD Dataset  
- Jupyter Notebook

---

##  Dataset

The project uses the **WESAD (Wearable Stress and Affect Detection)** dataset, which contains multimodal data (ECG, EDA, Respiration, etc.) collected from 15 subjects. For this project, only the ECG signal was used.

- **Sampling Rate:** 700 Hz  
- **Sensor Placement:** Chest (RespiBAN)  
- **Emotional States:** Baseline, Stress, Amusement

> Note: The dataset is publicly available from the [WESAD project repository](https://ubicomp.eti.uni-siegen.de/home/datasets/).

---

##  Workflow

1. **Data Loading**  
   Load the `.pkl` files for each subject and extract ECG signals.

2. **Signal Preprocessing**  
   Filter, segment, and normalize ECG data.

3. **Feature Extraction**  
   Compute HRV-based features (time and frequency domain).

4. **Model Training**  
   Train classifiers (e.g., Random Forest) on labeled features.

5. **Evaluation**  
   Evaluate using confusion matrix, classification report, and visualization.

---

##  Models Used

- Random Forest Classifier  
- Other models like Logistic Regression and SVM can be added as future work.

---

##  Results

- Visualization of ECG signal patterns under different emotional states  
- Feature distributions show clear separation between classes  
- Models evaluated with precision, recall, and F1-score metrics

---

##  How to Run

1. Clone the repository  
2. Download the WESAD dataset and place `.pkl` files in a `data/` folder  
3. Open the notebook:  
