Here’s a professional and detailed **README** for your GitHub repository, written to showcase *you (Mohamad Lebdeh)* as the lead contributor and emphasize your technical and analytical work. It reads cleanly for recruiters, professors, or collaborators reviewing your profile.

---

# Exercise Tracking Project

### Exploring the Most Effective Models for Exercise Recognition and Repetition Tracking

**Prepared by:** Mohamad Lebdeh
**Collaborators:** Matin Rahmani Neishabour, Mostafa Aboutaam, Arturo Rebolledo
**Advisor:** Dr. Tim H. Lin
**Institution:** California State Polytechnic University, Pomona

---

## Overview

This project investigates the use of **wearable sensors** (accelerometers and gyroscopes) for **tracking strength training exercises**. It focuses on building **machine learning models** that can recognize exercise types, count repetitions, and detect improper form using data collected from wrist-mounted devices.

The goal is to simulate the functionality of a **personal trainer** by applying advanced data processing and supervised learning techniques to wearable sensor data.

---

## Mohamad’s Role and Contributions

As the **Data Processing Lead** and a core developer, I was responsible for:

* Implementing Python scripts to **clean, preprocess, and filter raw sensor data**.
* Designing **noise reduction algorithms** using **Butterworth low-pass filtering**.
* Performing **feature engineering** through **Principal Component Analysis (PCA)** and **Fourier Transform**.
* Building and refining **predictive models** (Neural Network, Random Forest, KNN, Decision Tree, Naive Bayes).
* Conducting **accuracy evaluations** and producing **confusion matrices** for visual performance analysis.
* Writing modular, efficient Python code inside **Google Colab** and collaborating through shared notebooks.

My main objective was to enhance the **data reliability** and **model accuracy** across multiple participants and exercises.

---

## Project Architecture

**Platform Used:** Google Colab (Python 3)

**Core Tools and Libraries:**

* NumPy, Pandas, Matplotlib, Seaborn
* Scikit-learn, TensorFlow
* MbientLab MetaMotion Sensor Kit
* Fast Fourier Transform (FFT)
* PCA and K-Means Clustering

---

## Workflow Summary

### 1. Data Collection

* Sensor data from **five participants** performing **barbell exercises**.
* Recorded accelerometer and gyroscope readings for **six activities**: Bench, Overhead Press, Squat, Deadlift, Row, and Rest.
* Each exercise contained multiple repetitions and intensity levels (light, medium, heavy).

### 2. Data Processing

* Combined 69,000+ data entries with synchronized timestamps.
* Applied **low-pass filtering** and **outlier detection** (Chauvenet’s Criterion).
* Used **PCA** to reduce dimensionality and highlight dominant movement patterns.
* Transformed sensor data to frequency domain with **Fourier Transform**.

### 3. Feature Engineering

* Created multiple feature sets:

  * Basic: raw accelerometer and gyroscope data
  * Squared, PCA, Frequency, and Temporal features
  * Cluster-based features (K-Means with k=5)

### 4. Predictive Modeling

* Evaluated multiple supervised learning algorithms.
* Best-performing models achieved **>99% classification accuracy** for exercise recognition.

### 5. Evaluation

* Built **confusion matrix heatmaps** to interpret model predictions visually.
* Verified model consistency across participants (A–E).

---

## Key Results

* **Accuracy:** 99.14% (best neural network configuration)
* **Dataset Size:** ~70,000 samples, 5 participants
* **Feature Sets:** 6 progressively richer feature configurations
* **Sensor Input:** 6-axis (3 accelerometer + 3 gyroscope)
* **Outcome:** Automated recognition of strength exercises with near-perfect precision

---

## Lessons Learned

* Real-world sensor data requires **extensive preprocessing** to be model-ready.
* Combining **frequency and time-domain features** significantly improves classifier accuracy.
* Team coordination and iterative experimentation were crucial for convergence and optimization.
* Model generalization can vary across participants, making participant-based testing essential.

---

## Future Improvements

* Integrate **real-time feedback** into a mobile app.
* Add **repetition counting** and **form correction** logic using time-series modeling.
* Expand dataset diversity to include different body positions and exercises.
* Deploy trained models into **wearable devices** for continuous fitness tracking.

---

## Repository Structure

```
Exercise-Tracker/
│
├── Tracking-Project.ipynb         # Core machine learning and preprocessing notebook
├── Exercise Tracking.pdf          # Full project report (academic submission)
├── README.md                      # Project overview and Mohamad’s documentation
└── data/                          # (Optional) Dataset folder (if shared)
```

---

## Acknowledgments

Special thanks to:

* **Dr. Tim Lin** for academic supervision and technical guidance.
* **Matin Rahmani Neishabour** for leading model training and clustering analysis.
* **Mostafa Aboutaam** for experiment setup and synchronization logic.
* **Arturo Rebolledo** for participant coordination and data collection support.

---

## Author

**Mohamad Lebdeh**
B.S. Computer Engineering, Cal Poly Pomona (2023)
Machine Learning & Software Engineering Enthusiast
Email: MohamadLebdeh7@gmail.com

---

Would you like me to make this version formatted specifically for GitHub’s display (with proper markdown headings, tables, and bold text preserved)? It’ll render cleaner with readable section spacing.
