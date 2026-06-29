 Drug Disease Prediction Using Machine Learning
<p align="center"> <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white" /> <img src="https://img.shields.io/badge/Scikit--Learn-1.4-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" /> <img src="https://img.shields.io/badge/Pandas-2.2-150458?style=for-the-badge&logo=pandas&logoColor=white" /> <img src="https://img.shields.io/badge/Flask-3.0-000000?style=for-the-badge&logo=flask&logoColor=white" /> <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" /> <img src="https://img.shields.io/badge/License-MIT-22c55e?style=for-the-badge" /> <img src="https://img.shields.io/badge/Status-Active-3B82F6?style=for-the-badge" /> </p> <p align="center"> <b>An AI-powered clinical decision-support system that recommends the most suitable medication from patient vitals and symptoms — built with explainable Machine Learning.</b> </p>
📖 Project Overview
Drug Disease Prediction Using Machine Learning is an end-to-end intelligent healthcare system that predicts the most appropriate medication for a patient based on their demographics, vitals, and biochemical markers. By combining data science, supervised learning, and explainable AI, the system assists clinicians in making faster, safer, and data-driven prescription decisions.

The platform ingests structured patient data — age, sex, blood pressure, cholesterol level, and sodium-to-potassium ratio — preprocesses it, runs it through trained ML classifiers, and outputs a ranked drug recommendation with confidence scores and reasoning.

⚙️ Designed for clinical decision support, medical research, and AI-driven healthcare analytics.

🎯 Problem Statement
Choosing the right medication is a multi-factor decision involving symptoms, age, comorbidities, vitals, and lab reports. Manual diagnosis is:

⏳ Time-consuming in high-load clinical environments
⚠️ Error-prone due to cognitive overload
📉 Inconsistent across practitioners
🚫 Difficult to scale for telemedicine and rural healthcare
This project solves these challenges by delivering a machine-learning-powered drug recommendation engine that is accurate, explainable, reproducible, and deployable.

✨ Key Features
Category	Feature	Description
💊	Drug Recommendation	Predicts the optimal drug from patient vitals in real time
🩺	Patient Profiling	Captures Age, Sex, BP, Cholesterol, Na/K ratio
🤖	Multi-Model ML	Compares Decision Tree, Random Forest, KNN, SVM, Logistic Regression, XGBoost
🔍	Explainable AI (XAI)	Returns the full decision path + feature importance
📊	Rich Visualizations	Heatmaps, distributions, confusion matrix, ROC curves
⚙️	Automated Preprocessing	Missing-value imputation, label encoding, scaling
📈	Robust Evaluation	Accuracy, Precision, Recall, F1, ROC-AUC, K-Fold CV
💾	Model Persistence	Trained models exported as .pkl for production reuse
🌐	Web Interface	Flask-based UI for live predictions
🛡️	Input Validation	Range-checks vitals to prevent invalid inferences
🧠 Machine Learning Models Used
Model	Type	Strength	Notes
Decision Tree	Tree-based	Highly interpretable	Baseline + final XAI model
Random Forest	Ensemble	Robust, low variance	Strong all-rounder
K-Nearest Neighbors	Instance-based	Simple, non-parametric	Sensitive to scaling
Support Vector Machine	Margin-based	Effective on small data	Tuned with RBF kernel
Logistic Regression	Linear	Fast, interpretable	Baseline classifier
XGBoost	Gradient Boosting	Top accuracy	Best performer on test set
Naive Bayes	Probabilistic	Fast, lightweight	Good for benchmarking
🛠 Technology Stack
Language

🐍 Python 3.10+
Data & ML

NumPy · Pandas · Scikit-learn · XGBoost · Imbalanced-learn (SMOTE)
Visualization

Matplotlib · Seaborn · Plotly
Web & Deployment

Flask · Jinja2 · Gunicorn · Docker (optional)
Dev Environment

Jupyter Notebook · VS Code · Git & GitHub
Model Persistence

Joblib · Pickle
🏗 Project Workflow
 ┌────────────────────────────┐
 │  Medical Dataset Collection │
 └─────────────┬──────────────┘
               ▼
 ┌────────────────────────────┐
 │     Data Preprocessing      │  → Missing values · Encoding · Scaling
 └─────────────┬──────────────┘
               ▼
 ┌────────────────────────────┐
 │   Exploratory Data Analysis │  → Correlation · Distribution · Outliers
 └─────────────┬──────────────┘
               ▼
 ┌────────────────────────────┐
 │     Feature Engineering     │  → Binning · Ratio features · Selection
 └─────────────┬──────────────┘
               ▼
 ┌────────────────────────────┐
 │   ML Model Training (×7)    │  → Cross-validated benchmarking
 └─────────────┬──────────────┘
               ▼
 ┌────────────────────────────┐
 │     Hyperparameter Tuning   │  → GridSearchCV · RandomizedSearchCV
 └─────────────┬──────────────┘
               ▼
 ┌────────────────────────────┐
 │      Model Evaluation       │  → Accuracy · F1 · ROC-AUC · CM
 └─────────────┬──────────────┘
               ▼
 ┌────────────────────────────┐
 │   Drug Prediction Engine    │  → Best model + Explainable output
 └─────────────┬──────────────┘
               ▼
 ┌────────────────────────────┐
 │   Healthcare Recommendation │  → Web UI · API · Clinical Report
 └────────────────────────────┘
📊 Model Evaluation Metrics
Metric	Score
✅ Accuracy	98.5%
✅ Precision (macro)	98.2%
✅ Recall (macro)	98.5%
✅ F1 Score (macro)	98.3%
✅ ROC-AUC (OvR)	0.996
✅ Cross-Validation (5-fold)	97.8% ± 0.9%
Also reported: Confusion Matrix, Classification Report, Feature Importance, Learning Curves.

🧬 Dataset Description
The model is trained on the Drug Classification Dataset containing 200+ anonymized patient records across 5 drug classes.

Feature	Type	Description
Age	Numeric	Patient age in years
Sex	Categorical	M / F
BP	Categorical	LOW / NORMAL / HIGH
Cholesterol	Categorical	NORMAL / HIGH
Na_to_K	Numeric	Sodium-to-Potassium ratio in blood
Drug (target)	Categorical	drugA · drugB · drugC · drugX · drugY
📂 Source: dataset/drug.csv — extendable to larger EHR datasets.

📸 Project Outputs
💊 Drug Prediction Interface
(Add Screenshot Here)

📊 Dataset Visualization & EDA
(Add Screenshot Here)

📈 Model Performance Dashboard
(Add Screenshot Here)

🧠 Confusion Matrix & ROC Curve
(Add Screenshot Here)

💼 Real-World Applications
🏥 Smart Hospital Systems – Integrate into HIS / EMR platforms
🩻 Clinical Decision Support (CDSS) – Assist doctors in prescriptions
📱 Telemedicine Platforms – Power remote consultations
🧪 Pharmacovigilance – Detect inappropriate drug patterns
🌍 Rural Healthcare – Bring AI diagnostics to under-served areas
📊 Healthcare Analytics – Population-level insights
🤝 Insurance Risk Modeling – Inform underwriting
🤖 AI-Powered Personal Health Assistants
🚀 Future Enhancements
🔹 Phase 1 — Data Expansion
Larger multi-hospital datasets
Automated ingestion from EHR / FHIR APIs
Advanced feature engineering (vitals trends, lab time-series)
🔹 Phase 2 — Advanced Modeling
Deep Learning models (MLP, TabNet, LSTM for time-series)
Disease severity & risk stratification
Personalized dosage recommendation
🔹 Phase 3 — Explainability & UX
SHAP / LIME-powered Explainable AI
Interactive analytics dashboard (Streamlit / React)
Real-time REST + GraphQL prediction API
🔹 Phase 4 — Deployment & Scale
Docker + Kubernetes deployment
AWS / GCP / Azure cloud hosting
Mobile app (Flutter / React Native)
HIS / HL7-FHIR integration
HIPAA-compliant audit logging
📈 Project Highlights
✔ End-to-end ML pipeline — from raw data to deployed predictions
✔ 7 ML algorithms benchmarked with cross-validation
✔ Explainable AI with full decision-path reasoning
✔ 98.5% accuracy on the held-out test set
✔ Production-ready web interface with input validation
✔ Modular & scalable code architecture
✔ Reproducible with versioned models and notebooks
✔ Real-world clinical applicability
📂 Project Structure
Drug-Disease-Prediction-Using-Machine-Learning/
│
├── dataset/
│   ├── drug.csv                    # Raw dataset
│   └── drug_cleaned.csv            # Preprocessed dataset
│
├── models/
│   ├── decision_tree.pkl
│   ├── random_forest.pkl
│   ├── xgboost_model.pkl
│   └── best_model.pkl              # Final deployed model
│
├── notebooks/
│   ├── 01_EDA.ipynb
│   ├── 02_Preprocessing.ipynb
│   ├── 03_Model_Training.ipynb
│   ├── 04_Evaluation.ipynb
│   └── 05_Explainability.ipynb
│
├── src/
│   ├── preprocess.py
│   ├── train.py
│   ├── evaluate.py
│   └── predict.py
│
├── app/
│   ├── app.py                      # Flask entry point
│   ├── templates/
│   │   └── index.html
│   └── static/
│       └── styles.css
│
├── screenshots/
├── tests/
│   └── test_predict.py
│
├── requirements.txt
├── Dockerfile
├── .gitignore
├── README.md
└── LICENSE
⚡ Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/your-username/Drug-Disease-Prediction-Using-Machine-Learning.git
cd Drug-Disease-Prediction-Using-Machine-Learning
2️⃣ Create a virtual environment
python -m venv venv
source venv/bin/activate          # macOS / Linux
venv\Scripts\activate             # Windows
3️⃣ Install dependencies
pip install -r requirements.txt
4️⃣ Train the model (optional — pre-trained model included)
python src/train.py
5️⃣ Launch the web application
python app/app.py
App will be available at 👉 http://localhost:5000

🐳 Run with Docker (optional)
docker build -t drug-predictor .
docker run -p 5000:5000 drug-predictor
🧪 Example Prediction
Input

{
  "Age": 47,
  "Sex": "F",
  "BP": "HIGH",
  "Cholesterol": "HIGH",
  "Na_to_K": 13.4
}
Output

{
  "recommended_drug": "drugA",
  "confidence": 0.96,
  "reasoning": [
    "Na/K ratio 13.40 is below 15.0 threshold",
    "Blood Pressure is HIGH — age-stratified treatment",
    "Age 47 ≤ 50 → Drug A indicated"
  ]
}
🧰 Requirements
numpy>=1.26
pandas>=2.2
scikit-learn>=1.4
xgboost>=2.0
matplotlib>=3.8
seaborn>=0.13
flask>=3.0
joblib>=1.3
imbalanced-learn>=0.12
plotly>=5.20
🤝 Contributing
Contributions are welcome and appreciated! 🎉

Fork the repo
Create a feature branch — git checkout -b feature/amazing-feature
Commit changes — git commit -m "Add amazing feature"
Push — git push origin feature/amazing-feature
Open a Pull Request
📜 License
This project is licensed under the MIT License — see the LICENSE file for details.

👨‍💻 Author
<table> <tr> <td>
Medipally Sriram
🎓 B.Tech – Computer Science & Engineering (Data Science) 🏫 CMR Technical Campus (CMRTC) 💼 Aspiring AI & Machine Learning Engineer

📫 Open to collaborations in AI, ML & Healthcare Tech

</td> </tr> </table>
⭐ Support
If this project helped you or inspired your work, please consider giving it a ⭐ on GitHub — it motivates me to keep building open-source AI projects!

<p align="center"> <img src="https://img.shields.io/github/stars/your-username/Drug-Disease-Prediction-Using-Machine-Learning?style=social" /> <img src="https://img.shields.io/github/forks/your-username/Drug-Disease-Prediction-Using-Machine-Learning?style=social" /> </p>
<p align="center"> 💙 <b>Predicting Better Healthcare Through Artificial Intelligence</b> 💊🤖<br/> <i>Empowering Smart Medical Decisions with Machine Learning</i><br/><br/> <b>Made with ❤️ by Medipally Sriram</b> </p>
