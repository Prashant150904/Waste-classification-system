# 🗑️ AI-Based Waste Classification System
### Final Year Project | SVIT Vasad | Computer Engineering

---

## 📌 What is This Project?

An AI-powered waste classification system that classifies waste into:
- 🌿 **Organic** — Food waste, leaves, wood
- ♻️ **Recyclable** — Plastic, metal, paper

It takes waste properties as input and predicts which bin to use.

---

## 📊 Dataset

- **Total Samples** : 2,527
- **Features**      : 6
- **Classes**       : 2 (Organic, Recyclable)

| Feature | What it means |
|---|---|
| Material Type | What the waste is made of |
| Weight (kg) | How heavy it is |
| Size (cm) | How big it is |
| Is Contaminated | Is it mixed with food/liquid |
| Moisture Level | How wet it is |
| Decompose Days | How many days to decompose |

---

## 🤖 Machine Learning Models

We trained 3 different AI models and compared them:

| Model | How it works | Accuracy |
|---|---|---|
| Decision Tree | Like a flowchart — asks yes/no questions | 89.5% |
| **Random Forest** ⭐ | 100 decision trees voting together | **92.5%** |
| Logistic Regression | Uses math formula to find probability | 92.1% |

**Random Forest was selected as the best model with 92.5% accuracy**

---

## 📈 Graphs Generated

| Graph | What it shows |
|---|---|
| Class Distribution | How many organic vs recyclable samples |
| Model Comparison | Which model performed best |
| Confusion Matrix | How many correct/wrong predictions |
| Feature Importance | Which property matters most for prediction |
| ROC Curve | How well model separates two classes |
| Feature Distributions | How each property differs between classes |
| Correlation Heatmap | How properties relate to each other |
| Results Table | Final accuracy summary of all models |

---

## 🌐 Flask Web Application

We built a website where anyone can:
- Enter waste details
- Click Classify Waste
- Get instant prediction

| Technology | Purpose |
|---|---|
| HTML | Structure of the webpage (like skeleton) |
| CSS | Design/styling of webpage (like clothes) |
| JavaScript | Makes webpage interactive (like brain) |
| Flask | Python connects ML model to website (like bridge) |

---

## 🔄 How the System Works
User enters Flask receives ML Model Result shown waste details → the data → predicts → on screen (on website) (in Python) (Random Forest) (Organic/Recyclable)


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

## 📁 Project Structure

WasteClassification_FYP/ │ ├── waste_classification.py # Main ML script ├── app.py # Flask Web App ├── save_model.py # Save trained model ├── templates/ │ └── index.html # Frontend UI ├── outputs/ # All 8 graphs ├── model/ # Saved ML models ├── requirements.txt # Python libraries ├── .gitignore # Git ignore file └── README.md # Project documentation

🚀 How to Run1. Clone RepositoryBashgit clone https://github.com/Kitz2004/WasteClassification-FYP.git
cd WasteClassification-FYP
2. Create Virtual EnvironmentBashpython -m venv .venv
.venv\Scripts\activate
3. Install RequirementsBashpip install -r requirements.txt
4. Train and Save ModelBashpython waste_classification.py
python save_model.py
5. Run Web AppBashpython app.py
6. Open BrowserPlaintexthttp://127.0.0.1:5000
📊 Final ResultsModelAccuracyPrecisionRecallF1-ScoreDecision Tree89.5%0.900.900.89Random Forest ⭐92.5%0.930.920.92Logistic Regression92.1%0.920.920.92✅ Project Achievements✅ Trained 3 ML models✅ Achieved 92.5% accuracy✅ Generated 8 analytical graphs✅ Built working web application✅ Uploaded to GitHub✅ Follows complete ML pipeline: Data Generation → Preprocessing → Training → Evaluation → Deployment📝 Project SummaryWe built an AI-based waste classification system as our Final Year Project. The system uses Machine Learning to classify waste into Organic and Recyclable categories. We trained 3 different ML models on 2,527 waste samples and found that Random Forest gave the best accuracy of 92.5%. We also built a web application using Flask where users can enter waste properties and get instant classification results. The project is deployed locally and uploaded to GitHub.

