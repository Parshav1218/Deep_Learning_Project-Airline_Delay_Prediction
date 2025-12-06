# ✈️ Airline Delay Prediction using Deep Learning (LSTM Classifier)

![Status](https://img.shields.io/badge/Project%20Status-Completed-brightgreen)
![Python](https://img.shields.io/badge/Python-3.10-blue)
![PyTorch](https://img.shields.io/badge/Framework-PyTorch-red)
![Dataset](https://img.shields.io/badge/Dataset-Kaggle%20Flight%20Delays-orange)

---

## 📌 Project Overview

Flight delays significantly affect airline operations, passenger satisfaction, and cost efficiency.  
This project builds a **Deep Learning model using LSTM + Embeddings** to predict if a flight will be delayed by more than 15 minutes.

✔ Dataset: US DOT airline delay data (Kaggle)  
✔ Binary classification — **Delayed vs On‑time**  
✔ Implemented using **PyTorch**

---

## 📂 Repository Structure

├── data/
│ ├── flights.csv
│ ├── airlines.csv
│ ├── airports.csv
├── models/
│ ├── best_lstm_airline.pt
├── notebooks/
│ ├── Airline_Delay_Training.ipynb
├── results/
│ ├── loss_curve.png
│ ├── accuracy_curve.png
│ ├── confusion_matrix.png
│ ├── roc_curve.png
├── docs/
│ ├── Final_Report.docx
│ ├── Presentation.pptx
│ ├── Literature_Survey.pdf
└── README.md
---

## 📊 Dataset Used

📌 **Source:** https://www.kaggle.com/datasets/usdot/flight-delays  

### Key features:
- Airline code
- Airport (origin & destination)
- Distance
- Scheduled departure & arrival time
- Date components (month, day, weekday)

### Target variable:
1 → Delayed (> 15 minutes)
0 → On‑time

---

## 🔧 Tools & Technologies

- Python 3.10  
- PyTorch  
- NumPy & Pandas  
- Scikit‑Learn  
- Matplotlib / Seaborn  
- Google Colab

---

## 🧠 Model Architecture Summary

- **Embedding layers** for categorical fields
- **LSTM sequence learning layer**
- **Fully connected dense layer for classification**
- **Softmax output**

Loss Function → CrossEntropyLoss  
Optimizer → Adam

---

## 🚀 How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/<username>/<repo-name>.git
cd <repo-name>

2. Install Dependencies
bash
Copy code
pip install -r requirements.txt
3. Add Dataset
Place:
  flights.csv  
  airlines.csv  
  airports.csv  
              inside /data/ folder.

4. Train / Evaluate Model
Run the notebook:
notebooks/Airline_Delay_Training.ipynb
📈 Model Performance
| Metric   | Score                               |
| -------- | ----------------------------------- |
| Accuracy | ~83–84%                             |
| ROC‑AUC  | ~0.75                               |
| F1‑Score | ~0.27 (affected by class imbalance) |


📉 Key Visual Outputs
✔ Training loss curve
✔ Validation accuracy curve
✔ Confusion matrix heatmap
✔ ROC curve

📚 Documentation
📄 Final Report → /docs/Final_Report.docx

🔮 Future Improvements
Add weather + airport congestion data
Try transformer or attention-based models
Deploy model as real‑time API
Improve class imbalance handling

👥 Contributors
Parshav Goyal
Charu Garg
Vaibhavi Kumari
vidisha
