# 📂 AI & Machine Learning Projects Portfolio

**Name:** Subhadeep Sarkar  

**Registration Number:** 23BAI10977

**Application Number:** IN26010913

**Batch Number:** 1A

**Email ID:** subhadeep.23bai10977@vitbhopal.ac.in 

---

A collection of **9 projects** spanning Machine Learning, Deep Learning, Computer Vision, Natural Language Processing, and Reinforcement Learning — built with Python, TensorFlow, Scikit-learn, Flask, and more.

---

## 📑 Projects at a Glance

| # | Project | Domain | Tech Highlights | Live Demo |
|---|---|---|---|---|
| 1 | [Adult Census Income Classification](./Adult%20Census%20Income%20Classification/) | ML — Classification | Logistic Regression, Decision Tree, Random Forest, KNN, SVM | — |
| 2 | [Cancer Classification (Brain Tumor MRI)](./Cancer%20Classification/) | DL — Medical Imaging | CNN, TensorFlow, ImageDataGenerator, 4-class MRI | — |
| 3 | [Car Price Prediction](./Car_Price_Prediction/) | ML — Regression | Random Forest, Flask, Pickle | [🌍 Live on Render](https://car-price-predictor-skgz.onrender.com/) |
| 4 | [CIFAR-10 Image Classification](./CIFAR%2010/) | DL — Computer Vision | CNN, Data Augmentation, BatchNorm | — |
| 5 | [LFW Face Recognition](./LFW%20Face%20Recognition/) | DL — Face Recognition | CNN, LFW Dataset, 7-class face ID | — |
| 6 | [Movie Recommendation System](./Movie%20Recommendation/) | ML — NLP / Recommender | TF-IDF, Cosine Similarity, Flask | — |
| 7 | [RAG Chatbot (Amazon 10-Q)](./RAG_ChatBot/) | NLP — RAG | FastAPI, FAISS, Gemini AI, Sentence-Transformers | [Live](https://rag-chatbot-zyr8.onrender.com/) |
| 8 | [CartPole (PPO)](./CartPole/) | RL — Control | Stable-Baselines3, PPO, Gymnasium | — |
| 9 | [Lunar Lander (DQN)](./Lunar%20Lander/) | RL — Control | Stable-Baselines3, DQN, Box2D | — |

---

## 🔬 Project Details

### 1. 💰 [Adult Census Income Classification](./Adult%20Census%20Income%20Classification/)

Predicts whether an individual's annual income exceeds **$50K** based on census data. Compares **5 classifiers** (Logistic Regression, Decision Tree, Random Forest, KNN, SVM) on metrics like Accuracy, Precision, Recall, F1, and ROC-AUC.

**Dataset:** Adult Census Income Dataset (Kaggle) — ~32,561 records, 14 features  
**Pipeline:** Data Cleaning → Feature Engineering (One-Hot, StandardScaler) → Model Training → Evaluation

---

### 2. 🧠 [Cancer Classification — Brain Tumor MRI](./Cancer%20Classification/)

Classifies brain MRI images into **4 categories** (Glioma, Meningioma, No Tumor, Pituitary) using a custom **3-block CNN** with BatchNorm, Dropout, and data augmentation. Targets **90%+ accuracy**.

**Dataset:** Brain Tumor MRI Dataset (Kaggle) — 5,600 training + 1,600 test images  
**Architecture:** 3 × Conv blocks (32→64→128) + GlobalAveragePooling + EarlyStopping

---

### 3. 🚗 [Car Price Prediction](./Car_Price_Prediction/)

Predicts the selling price of used cars using a **Random Forest Regressor**, deployed as a **Flask web app** on Render.

🌍 **Live Demo:** (https://car-price-predictor-skgz.onrender.com/)

**Dataset:** Vehicle Dataset from CarDekho (Kaggle) — ~301 records  
**Features:** Present Price, Kms Driven, Fuel Type, Transmission, Car Age, etc.  
**Deployment:** Flask + Pickle → Render

---

### 4. 🖼️ [CIFAR-10 Image Classification](./CIFAR%2010/)

Classifies **32×32 RGB images** into **10 object categories** (Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, Truck) using a custom CNN with data augmentation. Targets **85%+ accuracy**.

**Dataset:** CIFAR-10 — 50,000 training + 10,000 test images (loaded via TensorFlow)  
**Architecture:** 3 × Conv blocks (32→64→128) + Flatten + Dense + ReduceLROnPlateau

---

### 5. 👤 [LFW Face Recognition](./LFW%20Face%20Recognition/)

Recognizes **faces of 7 public figures** from the Labeled Faces in the Wild dataset using a custom CNN. Handles limited training data through augmentation and stratified splitting.

**Dataset:** LFW — 1,288 grayscale images (50×37), 7 classes (loaded via scikit-learn)  
**Architecture:** 3 × Conv blocks (32→64→128) + EarlyStopping (patience=20)

---

### 6. 🎬 [Movie Recommendation System](./Movie%20Recommendation/)

A content-based movie recommendation engine using **TF-IDF Vectorization** and **Cosine Similarity** on movie genres. Served through a clean **Flask web interface**.

**Dataset:** TMDB Movie Dataset  
**Pipeline:** TF-IDF on genres → Cosine Similarity matrix → Top-N recommendations

---

### 7. 🤖 [RAG Chatbot — Amazon Quarterly Report](./RAG_ChatBot/)

A Retrieval-Augmented Generation chatbot that answers questions about Amazon's 10-Q quarterly report, grounded in the actual filing text with **citations**.

🌍 **Live Demo:** https://rag-chatbot-zyr8.onrender.com/

**Stack:** FastAPI + Sentence-Transformers (MiniLM) + FAISS (vector search) + Gemini AI  
**Flow:** Embed query → FAISS similarity search → Top-k excerpts → Gemini generates grounded answer

---

### 8. 🎮 [CartPole — PPO Reinforcement Learning](./CartPole/)

Trains an agent to balance a pole on a cart using **Proximal Policy Optimization (PPO)** with Stable-Baselines3 in the Gymnasium CartPole-v1 environment.

**Framework:** Stable-Baselines3, Gymnasium  
**Components:** `train.py`, `evaluate.py`, `test.py`, `record_video.py`, `plot_training.py`

---

### 9. 🚀 [Lunar Lander — DQN Reinforcement Learning](./Lunar%20Lander/)

Trains an autonomous spacecraft agent to safely land on a designated pad using **Deep Q-Network (DQN)** with the Box2D physics simulator.

**Framework:** Stable-Baselines3, Gymnasium (LunarLander-v3)  
**Components:** `train.py`, `evaluate.py`, `test.py`, `record_video.py`, `plot_training.py`

---

## 🧰 Technologies Used

| Category | Tools & Libraries |
|---|---|
| **Languages** | Python 3 |
| **ML / DL** | Scikit-learn, TensorFlow / Keras |
| **RL** | Stable-Baselines3, Gymnasium |
| **NLP / RAG** | TF-IDF, Sentence-Transformers, FAISS, Gemini AI |
| **Web** | Flask, FastAPI |
| **Data** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **Deployment** | Render, Pickle |
| **Environment** | Jupyter Notebook, VS Code |

---

## 📁 Repository Structure

```
├── Adult Census Income Classification/   # ML classification (5 models)
├── Cancer Classification/                # CNN brain tumor MRI (4-class)
├── Car_Price_Prediction/                 # Random Forest + Flask web app
├── CIFAR 10/                             # CNN image classification (10-class)
├── LFW Face Recognition/                 # CNN face recognition (7-class)
├── Movie Recommendation/          # TF-IDF + Flask recommender
├── RAG ChatBot/                          # RAG chatbot with FAISS + Gemini
├── CartPole/                             # PPO reinforcement learning
├── Lunar Lander/                         # DQN reinforcement learning
└── README.md                             # This file
```

---
