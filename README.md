# 🫀 ECG Arrhythmia Classification using MIT-BIH Dataset


This project focuses on the classification of ECG arrhythmias using the **MIT-BIH Arrhythmia Database**. It includes end-to-end preprocessing of ECG signals, heartbeat labeling according to **AAMI standards**, feature extraction, and machine learning-based classification.

---

## 📦 Project Structure

| File                             | Description                                         |
|----------------------------------|-----------------------------------------------------|
| `Final_signals-preprocessing.ipynb` | Loads and processes ECG signals from MIT-BIH. Handles beat annotation and AAMI classification. |
| `MODELING.ipynb`                   | Performs training and evaluation of ML models on preprocessed ECG data. |

---

## 📊 Project Workflow

1. **📁 Data Collection**  
   Load ECG signals from **MIT-BIH Arrhythmia Database** using `wfdb`.

2. **🧹 Signal Preprocessing**  
   Remove noise, extract heartbeats, and classify beats using AAMI standards.

3. **📈 Feature Extraction**  
   Extract statistical or signal-based features (RR interval, amplitude, etc.).

4. **🤖 Modeling**  The models used include:

LSTM (Long Short-Term Memory)

GRU (Gated Recurrent Unit)

Hybrid Systems combining LSTM and GRU
  

5. **✅ Evaluation**  


---

## 🧬 Dataset

- **Source:** [MIT-BIH Arrhythmia Database](https://physionet.org/content/mitdb/1.0.0/)
- **Description:** Contains 48 half-hour ECG recordings annotated with heartbeat types.

---

## 🧠 AAMI Beat Classification

| Class | Beats Included                      | Meaning                        |
|-------|-------------------------------------|--------------------------------|
| N     | N, L, R, e, j, etc.                 | Normal                         |
| S     | A, a, J, S, etc.                    | Supraventricular ectopic       |
| V     | V, E, etc.                          | Ventricular ectopic            |
| F     | F                                   | Fusion                         |
| Q     | /, f, Q, ?                          | Unknown or unclassifiable      |

---

## 💻 Technologies Used

- **Language:** Python
- **Libraries:**
  - `wfdb` for ECG signal access
  - `pandas`, `numpy` for data handling
  - `scikit-learn` for modeling
  - `matplotlib`, `seaborn` for visualization

---

## 🛠️ Hardware Context

This project simulates ECG signal processing, but in real-time settings it can be integrated with (**UNDER IMPROVE MENT**):

- **ECG sensor modules** (like AD8232)
- **Raspberry Pi / Arduino** for acquisition
- **Cloud APIs** (Firebase / AWS) for real-time storage & access

---
