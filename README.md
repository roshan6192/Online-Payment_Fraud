# Online-Payment_Fraud

# 💳 Online Payment Fraud Detection (Streamlit + Docker)

This project is a real-time fraud detection web app built with **Streamlit**, based on a machine learning model trained on a financial transaction dataset.

It includes:
- Transaction type distribution visualization
- Correlation analysis
- Random Forest classifier training
- Interactive fraud prediction for new transactions
- Fully containerized using **Docker**

---

## 🧠 Dataset

The model uses the [Online Payment Fraud dataset](https://www.kaggle.com/datasets/ealaxi/paysim1) which includes features like:
- `step`, `amount`, `oldbalanceOrg`, `newbalanceOrig`, `oldbalanceDest`, `newbalanceDest`, `type`, and `isFraud`

Ensure the file `onlinefraud.csv` is placed in the same directory as `app.py`.

---

## 🚀 How to Run (Locally)

### ✅ 1. Clone the repository

```bash
git clone https://github.com/yourusername/online-payment-fraud.git
cd online-payment-fraud

### ✅ 2. Add the dataset
onlinefraud.csv

### ✅ 3. Install dependencies (without Docker)
pip install -r requirements.txt
streamlit run app.py

### 🐳 Run with Docker
### ✅ 1. Build Docker image
docker build -t fraud-app .

### ✅ 2. Run Docker container
docker run -p 8501:8501 fraud-app

### ✅ 3. Clone the repository
docker run -p 8501:8501 fraud-app
