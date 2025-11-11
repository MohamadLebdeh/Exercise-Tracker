# Exercise Tracking Project

### Exploring Machine Learning Models for Exercise Recognition and Repetition Tracking

**Author:** Mohamad Lebdeh
**Collaborators:** Matin Rahmani Neishabour, Arturo Rebolledo
**Advisor:** Dr. Tim H. Lin
**Institution:** California State Polytechnic University, Pomona

---

## Overview

This project applies **wearable sensor data** from accelerometers and gyroscopes to automatically recognize **strength training exercises**, **count repetitions**, and **identify improper form**.
It demonstrates how machine learning and signal processing can simulate aspects of a **personal trainer** by analyzing motion patterns captured from wrist-mounted sensors.

The work focuses on end-to-end data handling—from **raw sensor acquisition** to **model evaluation**—and uses multiple supervised learning algorithms to identify optimal architectures for human activity recognition.

---

## Mohamad’s Role and Contributions

As the **Data Processing Lead** and a primary developer, I focused on ensuring the reliability and accuracy of the full data pipeline:

* Built Python scripts to **clean, synchronize, and preprocess raw accelerometer and gyroscope data**.
* Designed **noise-reduction algorithms** using **Butterworth low-pass filtering** and outlier detection.
* Engineered features with **Principal Component Analysis (PCA)** and **Fast Fourier Transform (FFT)** to extract both time- and frequency-domain characteristics.
* Trained and optimized **Neural Network**, **Random Forest**, **K-Nearest Neighbors**, **Decision Tree**, and **Naive Bayes** models.
* Conducted **performance evaluation** using confusion matrices, cross-validation, and model comparison charts.
* Wrote modular, well-documented Python code in **Google Colab** and managed shared collaborative notebooks.

---

## Project Architecture

**Platform:** Google Colab (Python 3)

**Core Tools and Libraries:**

* NumPy, Pandas, Matplotlib, Seaborn
* Scikit-learn, TensorFlow
* MbientLab MetaMotion Sensor Kit
* PCA, FFT, K-Means Clustering

---

## Workflow Summary

### 1. Data Collection

* Captured multi-axis sensor data from **five participants** performing six barbell exercises: Bench Press, Overhead Press, Squat, Deadlift, Row, and Rest.
* Each participant performed multiple repetitions across light, medium, and heavy intensities.

### 2. Data Processing

* Combined and synchronized **69,000+ time-series entries**.
* Applied **low-pass Butterworth filtering** to reduce high-frequency noise.
* Detected and removed outliers using **Chauvenet’s Criterion**.
* Used **PCA** for dimensionality reduction and feature selection.
* Converted signals to the frequency domain via **Fourier Transform**.

### 3. Feature Engineering

* Built progressive feature sets:

  * Raw accelerometer and gyroscope data
  * Squared, PCA-based, and frequency features
  * Cluster-derived features using **K-Means (k=5)**

### 4. Predictive Modeling

* Compared multiple supervised algorithms.
* Best models (Neural Network and Random Forest) achieved **>99% classification accuracy** for exercise recognition.

### 5. Evaluation

* Generated **confusion matrices** and **accuracy comparisons** to visualize results.
* Validated model generalization across all participants (A–E).

---

## Key Results

* **Accuracy:** 99.14% (Neural Network)
* **Dataset Size:** ~70,000 samples, 5 participants
* **Features Tested:** 6 distinct engineered sets
* **Sensor Input:** 6-axis (3 accelerometer + 3 gyroscope)
* **Outcome:** Highly reliable model for exercise recognition and rep tracking

---

## Lessons Learned

* Real sensor data requires **extensive preprocessing** before modeling.
* Blending **frequency-domain and time-domain features** significantly boosts accuracy.
* Team iteration and experimental validation are key to optimizing results.
* Generalization varies by subject, reinforcing the value of participant-based validation.

---

## Future Improvements

* Integrate **real-time classification** into a mobile application.
* Add **automatic rep counting** and **form correction** via time-series modeling.
* Expand dataset diversity with additional exercises and participants.
* Deploy trained models on **wearable devices** for live feedback.

---

## Repository Structure

```
Exercise-Tracker/
│
├── Tracking-Project.ipynb      # Main ML and preprocessing notebook
├── Exercise Tracking.pdf       # Full academic report
├── README.md                   # Project overview and documentation
└── data/                       # (Optional) Dataset folder
```

---

## Acknowledgments

Special thanks to:

* **Dr. Tim H. Lin** – Faculty advisor and project mentor
* **Matin Rahmani Neishabour** – Lead model training and clustering analysis
* **Mostafa Aboutaam** – Experiment setup and data synchronization
* **Arturo Rebolledo** – Participant coordination and data collection

---

## Author

**Mohamad Lebdeh**
B.S. Computer Engineering, Cal Poly Pomona (2023)
Machine Learning & Software Engineering Enthusiast
Email: [MohamadLebdeh7@gmail.com](mailto:MohamadLebdeh7@gmail.com)
