# 🏠 Task 3: Multimodal House Price Classification

## 📌 Overview
This project was completed as part of the **AI/ML Engineering Internship** at DevelopersHub Corporation.  
The goal was to build a **multimodal deep learning model** that predicts house price categories using both **tabular data** and **house images**.

## 🎯 Objective
Predict 5 price categories:
- **Budget** ($0 - $300,000)
- **Economy** ($300,000 - $500,000)
- **Standard** ($500,000 - $700,000)
- **Premium** ($700,000 - $1,000,000)
- **Luxury** ($1,000,000+)

## 🏆 Results

| Metric | Score |
|--------|-------|
| **Accuracy** | **100%** |
| Target | 95% |
| Status | ✅ Exceeded |

### Per-Class Performance
| Category | Accuracy |
|----------|----------|
| Budget | 100% |
| Economy | 100% |
| Standard | 100% |
| Premium | 100% |
| Luxury | 100% |

## 🏗️ Model Architecture
┌─────────────────┐
│ HOUSE DATA │
└─────────┬───────┘
│
┌─────────────────┼─────────────────┐
│ │ │
▼ ▼ ▼
┌───────────────┐ ┌─────────────┐
│ ResNet50 │ │ MLP │
│ (Image) │ │ (Tabular) │
└───────┬───────┘ └──────┬──────┘
│ │
▼ ▼
[2048-dim] [64-dim]
│ │
└────────┬─────────┘
▼
┌─────────────────┐
│ Fusion │
│ (Concatenate) │
└────────┬────────┘
▼
┌─────────────────┐
│ Classifier │
│ 256 → 128 → 5 │
└────────┬────────┘
▼
[Price Category]

## 📊 Visualizations

### Confusion Matrix
![Confusion Matrix](screenshots/confusion_matrix.png)

### Training Progress
![Training Curves](screenshots/training_curves.png)

## 🛠️ Technologies Used

| Category | Technologies |
|----------|--------------|
| Framework | PyTorch, torchvision |
| Model | ResNet50 (pretrained) |
| Data Processing | pandas, numpy, scikit-learn |
| Visualization | matplotlib, seaborn |
| Platform | Kaggle (GPU P100) |

## 📁 Repository Structure
├── Task3_Notebook.ipynb # Complete implementation
├── best_classifier.pth # Trained model weights
├── task3_results.txt # Performance metrics
├── scaler.pkl # Feature scaler
├── requirements.txt # Dependencies
└── README.md # This file

## 🚀 How to Run

1. **Clone the repository**
```bash
git clone https://github.com/YOUR_USERNAME/AI-ML-Internship-Task3-Multimodal.git
cd AI-ML-Internship-Task3-Multimodal


⭐ Star this repository if you found it useful!
