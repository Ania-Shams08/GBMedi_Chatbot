# 🏥 GB-MediBot: Medical Test Recommendation System Using Patient Symptoms

GB-MediBot is an AI-powered medical test recommendation system that predicts diseases from patient symptom descriptions and recommends appropriate medical tests. The project uses the **BERT (Bidirectional Encoder Representations from Transformers)** model for natural language understanding and multi-class disease classification.

> **Note:** This project is intended for educational and research purposes only. It is not a substitute for professional medical advice or diagnosis.

---

## 📌 Features

- Predicts diseases from patient symptom descriptions.
- Recommends relevant medical tests.
- Uses the pre-trained BERT transformer model.
- Handles natural language input from users.
- Performs multi-class disease classification (30 diseases).
- Includes data preprocessing, visualization, model training, and evaluation.

---

## 🛠️ Technologies Used

- Python
- TensorFlow
- Hugging Face Transformers
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab / Jupyter Notebook

---

## 📂 Dataset

The dataset was obtained from **Kaggle**.

**Dataset Information**
- Total Records: **1,498**
- Disease Classes: **30**
- Columns:
  - Questions (Patient Symptoms)
  - Medical Tests
  - Predicted Disease

---

## 📊 Project Workflow

1. Import required libraries.
2. Load the dataset.
3. Explore and clean the data.
4. Perform Exploratory Data Analysis (EDA).
5. Encode disease labels.
6. Tokenize symptom text using BERT Tokenizer.
7. Split the dataset into training and testing sets.
8. Build the BERT classification model.
9. Train the model with Early Stopping.
10. Evaluate using accuracy, confusion matrix, precision, recall, and F1-score.
11. Save the trained model.
12. Predict diseases and recommend medical tests.

---

## 🧠 Model Architecture

The project uses **BERT (Bidirectional Encoder Representations from Transformers)** for text classification.

### Model Pipeline

```
Patient Symptoms
        │
        ▼
BERT Tokenizer
        │
        ▼
Input IDs + Attention Masks
        │
        ▼
Pre-trained BERT Model
        │
        ▼
Classification Layer
        │
        ▼
Predicted Disease
        │
        ▼
Recommended Medical Test
```

---

## 📈 Evaluation Metrics

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

Training and validation curves were also plotted to monitor model performance.

---

## 📁 Project Structure

```
GB-MediBot/
│
├── dataset/
│   └── symptoms_based_medical_test_recommendations.csv
│
├── notebooks/
│   └── GB_MediBot.ipynb
│
├── model/
│   └── medical_tests_model.h5
│
├── images/
│   ├── confusion_matrix.png
│   ├── accuracy_curve.png
│   └── loss_curve.png
│
├── report/
│   └── GB_MediBot_Project_Report.pdf
│
├── README.md
└── requirements.txt
```

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/GB-MediBot.git
cd GB-MediBot
```

Install the required packages:

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

Run the notebook:

```bash
jupyter notebook
```

or open the project in **Google Colab** and execute all cells.

---

## 💡 Example

**Input**

```
I have a severe headache, fever, and body pain.
```

**Output**

```
Predicted Disease: Dengue

Recommended Medical Test:
Complete Blood Count (CBC)
NS1 Antigen Test
```

---

## 📌 Future Improvements

- Add more diseases and medical tests.
- Increase dataset size.
- Deploy as a web application.
- Develop a mobile application.
- Support multiple languages.
- Integrate with hospital databases.

---

## ⚠️ Disclaimer

This project is designed for educational and research purposes only. The predictions should not be considered medical advice or a replacement for consultation with qualified healthcare professionals.

---

## 👩‍💻 Author

**Ania Shams**

BS Computer Science  
Karakoram International University (KIU)

---

## 📜 License

This project is licensed under the MIT License.
