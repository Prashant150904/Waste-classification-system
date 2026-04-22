
# 🗑️ AI-Based Waste Classification System
### Final Year Project | SVIT Vasad | Computer Engineering

An AI-powered web application that classifies waste into **Organic** or **Recyclable** categories based on its physical properties. Built with Python, scikit-learn, and Flask.

---

## ✨ Key Features
* **Machine Learning Pipeline:** Trains and evaluates 3 models (Decision Tree, Random Forest, Logistic Regression).
* **High Accuracy:** Uses a tuned **Random Forest** model achieving ~92.5% classification accuracy.
* **Feature Analysis:** Evaluates waste based on 6 attributes (Material Type, Weight, Size, Contamination, Moisture, Decomposition Days).
* **Interactive UI:** A modern, responsive Flask web dashboard for real-time predictions and confidence scoring.
* **Automated Analytics:** Generates 8 detailed EDA and performance graphs (ROC curves, Feature Importance, Confusion Matrices).

---

## 🛠️ Tech Stack
* **Machine Learning:** `scikit-learn`, `pandas`, `numpy`
* **Visualization:** `matplotlib`, `seaborn`
* **Web Framework:** `Flask`
* **Frontend:** HTML5, CSS3, JavaScript

---

## 🚀 Quick Start Guide

### 1. Setup Environment
Clone the repository and install the required dependencies.
```bash
git clone :https://github.com/Prashant150904/Waste-classification-system.git

# Create and activate virtual environment
python -m venv .venv
.venv\Scripts\activate      # On Windows
# source .venv/bin/activate # On Mac/Linux

# Install packages
pip install -r requirements.txt
```

### 2. Train the Model & Generate Graphs
Run the main ML script to generate the dataset, train the models, and output the analysis graphs to the `outputs/` folder.
```bash
python waste_classification.py
```

### 3. Save the Production Model
Serialize the trained Random Forest model and encoders to the `model/` directory for the web app to use.
```bash
python save_model.py
```

### 4. Launch the Web Application
Start the Flask server and interact with the AI model in your browser.
```bash
python app.py
```
Open **`http://127.0.0.1:5000`** in your web browser.

---

## 📁 Project Structure
```text
WasteClassification-FYP/
├── app.py                    # Flask Web Application
├── waste_classification.py   # Main ML training & visualization script
├── save_model.py             # Script to export the .pkl model files
├── templates/
│   └── index.html            # Web Dashboard UI
├── outputs/                  # Generated analytical graphs
├── model/                    # Saved ML models and scalers
├── requirements.txt          # Python dependencies
└── README.md                 # Project documentation
```

---

## 💾 Project Files

| File | Purpose |
|---|---|
| `waste_classification.py` | Trains all 3 ML models and saves graphs |
| `save_model.py` | Saves trained model to disk |
| `app.py` | Runs the Flask website |
| `templates/index.html` | The webpage (HTML + CSS + JS) |
| `requirements.txt` | List of Python libraries needed |
| `outputs/` | All 8 graphs saved here |
| `model/` | Saved ML model files |

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| scikit-learn | Machine learning library |
| pandas | Data handling |
| numpy | Mathematical calculations |
| matplotlib & seaborn | Graph generation |
| Flask | Web application framework |
| HTML/CSS/JS | Frontend website |
| GitHub | Code storage and sharing |

---

📊 Final Results
Model	Accuracy	Precision	Recall	F1-Score
Decision Tree	89.5%	0.90	0.90	0.89
Random Forest ⭐	92.5%	0.93	0.92	0.92
Logistic Regression	92.1%	0.92	0.92	0.92


Project Summary
We built an AI-based waste classification system as our Final Year Project. The system uses Machine Learning to classify waste into Organic and Recyclable categories. We trained 3 different ML models on 2,527 waste samples and found that Random Forest gave the best accuracy of 92.5%. We also built a web application using Flask where users can enter waste properties and get instant classification results. The project is deployed locally and uploaded to GitHub.

---

## 👨‍💻 Developer

| Field | Detail |
| :--- | :--- |
| **Name** | Panchasara Prashant |
| **ID** | 22BECEG034 |
| **Email** | [panchasaraprashant4@gmail.com](mailto:panchasaraprashant4@gmail.com) |
| **College** | SVIT Vasad |
| **Department** | Computer Engineering |
```
