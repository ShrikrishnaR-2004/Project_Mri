
# 🎵 Maintenance and Preservation of Mridangam Using Machine Learning

This repository presents a machine learning-based approach for evaluating the condition of the **Mridangam**, a traditional South Indian percussion instrument. Our project uses acoustic signal analysis and classification to assist in automated diagnostics, aiding musicians and instrument makers in preserving the tonal quality and structural integrity of the Mridangam.

## 📌 Overview

Traditional Mridangam maintenance is subjective and labor-intensive, relying on the artisan's experience. This project introduces a **Support Vector Machine (SVM)** classifier trained on **Mel-Frequency Cepstral Coefficients (MFCCs)** and other audio features to determine the instrument's condition based on recorded audio strokes.

> 🔍 Conditions classified:
- **Good** – Well-tuned, structurally sound
- **Needs Tuning** – Minor tonal inconsistencies
- **Needs Maintenance** – Structural or acoustic deterioration

## 🧠 Tech Stack

- **Python 3**
- **Librosa** – Audio processing and feature extraction
- **Scikit-learn** – SVM classifier, model training & evaluation
- **NumPy, Pandas, Matplotlib** – Data handling and visualization

## 🔁 Project Workflow

1. **🎙 Audio Data Collection**
   - Record strokes (`tha`, `dhin`, `nam`, `chappu`, `gumki`) from Mridangams in different conditions.
   - Label audio samples based on expert evaluation.

2. **⚙️ Preprocessing & Feature Extraction**
   - Extract MFCCs, Spectral Centroid, Bandwidth, Flatness, RMS Energy.
   - Normalize and frame the features for model input.

3. **🧪 Model Training & Validation**
   - Use SVM for classification.
   - Split data into train/test sets.
   - Perform cross-validation to avoid overfitting.

4. **📊 Evaluation**
   - Achieved **77% Accuracy**
   - High precision and recall in detecting "Good" instruments.
   - Use of confusion matrix to identify classification bottlenecks.

5. **🚀 Deployment**
   - Build an inference pipeline that takes audio input and returns condition classification.
   - Potential to extend as a mobile or desktop application.

## 📈 Results

| Condition           | Precision | Recall |
|---------------------|-----------|--------|
| Good                | 0.81      | 0.96   |
| Needs Tuning        | 0.80      | 0.32   |
| Needs Maintenance   | 0.66      | 0.67   |

- The model is highly accurate for detecting well-maintained instruments.
- Some overlap occurs between "Needs Tuning" and "Needs Maintenance" due to subtle acoustic similarities.


## 📚 Research Paper

You can read the full research paper here: https://doi.org/10.56975/ijsdr.v10i4.302361

## 🧪 Future Improvements

- Expand dataset with more diverse playing conditions and instruments.
- Explore deep learning models (CNNs, Transformers) for better accuracy.
- Integrate real-time audio input for mobile apps.
- Collaborate with artisans to improve subjective tuning classification.

## 👥 Authors

- Shrikrishna R

📧 Contact: rshrikrishna84@gmail.com

---

> 🎯 *Empowering traditional musicians with intelligent tools to preserve India's musical heritage.*
