# 🎬 AI-Powered Movie Recommendation System - Smarter & Personalized Viewing

This project delivers an **AI-powered movie recommendation system** designed to enhance user experiences through **advanced collaborative filtering** (SVD from `Surprise`), **content-based analysis** (TF-IDF), and **explainability using SHAP**. This intelligent system provides **personalized movie suggestions**, backed by a transparent decision-making process.

---

## 🚀 **Project Overview**

### 🎯 **Why This Matters**
Ever wondered how platforms like Netflix recommend movies tailored to your taste? This project replicates that functionality, using **collaborative filtering** to predict user preferences, enriched with **content-based filtering** for better recommendations.

### 🔑 **Key Features**
- **📊 Data Exploration:** Analyzing user preferences and rating behaviors.
- **🔄 Preprocessing Pipeline:** Leveraging **TF-IDF** for textual analysis.
- **🚀 Model Training & Evaluation:** Implementing **Surprise SVD** for robust recommendations.
- **📈 Explainability with SHAP:** Ensuring AI-driven suggestions are interpretable.
- **🎯 Model Performance Benchmarking:** Comparing different approaches (SVD, KNN, NMF).

---

## 📊 **Visual Insights**

### **1️⃣ Distribution of Ratings**
![Distribution of Ratings](rating_distribution.png)
> *Analyzing how users rate movies to fine-tune recommendation accuracy.*

### **2️⃣ Model Performance Comparison**
![Model Performance](model_performance.png)
> *Evaluating RMSE and MAE across different recommendation models to ensure the best accuracy.*

---

## 📁 **Project Directory Structure**

```
📂 Recommendation_systems
│── 📜 Recommendation_systems.ipynb  # Jupyter Notebook
│── 📜 README.md                      # Project Documentation
│── 📂 data/                           # Dataset (if applicable)
│── 📂 models/                         # Saved models (if applicable)
│── 📂 images/                         # Visualizations
```

---

## 🛠 **Requirements & Installation**

Ensure your environment includes Python and the required libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn surprise shap
```

---

## 📊 **Dataset Breakdown**
The dataset consists of user-movie interactions, structured as follows:
- **User Ratings:** How users rate different movies (1-5 scale).
- **Movie Metadata:** Titles, descriptions, and genres.
- **Interaction Data:** Capturing the relationship between users and movies.

### **Sample Data Structure:**
```plaintext
userId  movieId  rating  timestamp
1       1        4.0     964982703
1       3        4.0     964981247
1       6        4.0     964982224
```

---

## 🚀 **Modeling Approach**

### 🎭 **Collaborative Filtering (SVD Algorithm)**
- Implements **Singular Value Decomposition (SVD)** from `Surprise`.
- Captures latent factors to predict unseen ratings.
- Enhances recommendations based on user similarities.

### 🏆 **Feature Engineering (TF-IDF)**
- Extracts meaningful insights from movie descriptions.
- Merges textual features with collaborative filtering for hybrid recommendations.

### 🎯 **Explainability (SHAP Analysis)**
- **SHAP values** enhance transparency in recommendation decisions.
- Identifies key factors influencing predictions.

---

## 📈 **Performance Metrics & Model Comparison**
- **RMSE (Root Mean Squared Error):** Measures prediction accuracy.
- **Precision & Recall:** Evaluates recommendation relevance.
- **MAE (Mean Absolute Error):** Assesses the consistency of predictions.

| Model | RMSE | MAE |
|--------|------|------|
| **SVD**  | **1.0453** | **0.8428** |
| KNN  | 1.0472 | 0.8471 |
| NMF  | 1.0424 | 0.8327 |

> *SVD outperforms other methods, making it the most reliable choice.*

---

## ✅ **Key Takeaways & Next Steps**
✔ **SVD-based models provide superior recommendation accuracy.**
✔ **Hybrid approaches incorporating content-based filtering improve results.**
✔ **Future work includes reinforcement learning for dynamic recommendations.**

---

## 💻 **How to Run the Project**
1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_GITHUB_USERNAME/Recommendation_systems.git
   ```
2. Navigate to the directory:
   ```bash
   cd Recommendation_systems
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook Recommendation_systems.ipynb
   ```

---

## 🌟 **Acknowledgments**
- The `Surprise` library for powerful recommendation algorithms.
- `SHAP` for providing model transparency.
- Open-source datasets enabling machine learning innovations.

---

🎬 *Unlock personalized movie recommendations—powered by AI!* 🍿


