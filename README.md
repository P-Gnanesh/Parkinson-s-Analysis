# 🧠 Parkinson’s Disease Prediction using SVM

This project uses **machine learning** to detect **Parkinson’s disease** from **biomedical voice measurements**.  
The model analyzes subtle vocal changes that are often early indicators of the disease, helping in faster and more accurate diagnosis.

---

## 📁 Dataset Overview

- **Name:** Parkinson’s Disease Dataset  
- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/parkinsons)  
- **Type:** Biomedical voice data  
- **Samples:** 195 voice recordings from 31 individuals  
- **Target Variable:** `status`  
  - `1` → Patient with Parkinson’s  
  - `0` → Healthy individual  

### 🗣️ About the Features
Each sample contains **voice features** (acoustic parameters) extracted from sustained phonation (saying “aaaah”).  
These features describe:
- **Frequency and pitch** (`MDVP:Fo(Hz)`, `MDVP:Fhi(Hz)`, `MDVP:Flo(Hz)`)  
- **Jitter & Shimmer** — small variations in frequency and loudness  
- **Noise ratios** (`NHR`, `HNR`) — indicate breathiness or instability in the voice  
- **Nonlinear measures** (`RPDE`, `DFA`, `PPE`) — capture complex patterns in vocal dynamics  

These characteristics help identify the subtle vocal changes associated with Parkinson’s.

---

## 🧩 Tools and Libraries Used

| Library | Purpose |
|----------|----------|
| **pandas** | Data loading and preprocessing |
| **numpy** | Numerical computations |
| **scikit-learn (sklearn)** | Building and evaluating the SVM model |

---

## ⚙️ Machine Learning Model

- **Algorithm Used:** Support Vector Machine (SVM)  
- **Goal:** Classify whether a person has Parkinson’s disease based on voice features  
- **Accuracy Achieved:** **88%**  
- **Steps Involved:**
  1. Load and clean dataset  
  2. Split into training and testing sets  
  3. Scale features for uniformity  
  4. Train SVM classifier  
  5. Evaluate model accuracy  

---

## 📊 Results

- **Model Accuracy:** 88%  
- The SVM model successfully distinguishes between healthy and Parkinson’s-affected voices.  
- Results indicate that **biomedical voice analysis** can be a valuable non-invasive tool for early detection.

---

## 🧠 Future Scope

- Experiment with other ML algorithms like Random Forest, Logistic Regression, or Neural Networks  
- Use larger and more diverse datasets  
- Develop a simple app interface for voice-based Parkinson’s screening  

---

## 🙌 Acknowledgment

Dataset provided by the **UCI Machine Learning Repository**  
Voice data recorded and analyzed by **Max Little et al.**

