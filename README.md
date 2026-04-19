<div align="center">

# 🌾 Fertilizer Prediction System

### *AI-Powered Smart Agriculture for Better Crop Yields*

[![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-2.x-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)](https://github.com/)
[![License](https://img.shields.io/badge/License-The_Unlicened-yellow?style=for-the-badge)](LICENSE)

<br/>

> *Empowering farmers with data-driven fertilizer recommendations — right soil nutrition, right crop, right time.*

</div>



##  About the Project

This project is a machine learning-based web application that predicts the most suitable fertilizer for crops based on user inputs such as Nitrogen, Phosphorous, Potassium levels, temperature, humidity, moisture, soil type, and crop type. It integrates real-time temperature data using the **OpenWeather API** and uses trained ML models to provide accurate, fast, and reliable fertilizer recommendations — helping farmers make smarter agricultural decisions.



##  Features

| Feature | Description |
|--------|-------------|
|  **Web Interface** | Clean, responsive UI for easy interaction |
|  **Real-Time Temperature** | Fetches live temperature data via OpenWeather API |
|  **ML Predictions** | Recommends the best fertilizer based on soil & environmental data |
|  **Fast & Accurate** | Powered by a pre-trained Naive Bayes model for quick predictions |
|  **Responsive Design** | Works seamlessly across devices |

---

##  Technologies Used

- **Backend:** Python, Flask
- **Machine Learning:** Scikit-learn (Decision Tree, Random Forest, Naive Bayes)
- **External API:** OpenWeather API (real-time temperature)
- **Frontend:** HTML5, CSS3
- **Model Serialization:** Pickle (`.pkl` files)

---

##  Machine Learning Models

Three classification models were trained and evaluated:

| Model | Description | Selected |
|-------|-------------|----------|
|  Decision Tree Classifier | Simple, interpretable tree-based model | No |
|  Random Forest Classifier | Ensemble of decision trees for better accuracy | No |
|  **Naive Bayes** | Probabilistic classifier — chosen for **highest accuracy** | Yes |

> **Final Model:** Naive Bayes Classifier — selected based on highest evaluation accuracy on the test dataset.

---

## 📂 Folder Structure

```
Fertilizer-Prediction-System/
│
├── static/                  # Static assets
│   ├── css/                 # Stylesheets
│   └── images/              # Project images & icons
│
├── templates/               # HTML templates (Jinja2)
│   ├── index.html           # Home / Input form page
│   └── result.html          # Prediction result page
│
├── App1.py                  #  Main Flask application
│
├── model.pkl                # Trained Naive Bayes model
├── fertilizer_encoder.pkl   # Label encoder for fertilizer names
├── soil_encoder.pkl         # Label encoder for soil types
├── crop_encoder.pkl         # Label encoder for crop types
│
├── fertilizer_data.csv      # Dataset used for training
├── Fertilizer_Prediction.ipynb  # Jupyter Notebook (EDA + Model Training)
│
├── requirements.txt         # Python dependencies
└── README.md                # Project documentation
```

---

##  Dataset

| Detail | Info |
|--------|------|
|  **Source** | [[Dataset Link](https://www.kaggle.com/code/pazindushane/fertilizers-recommendation/input)] |
|  **Features** | Nitrogen, Phosphorous, Potassium, Temperature, Humidity, Moisture, Soil Type, Crop Type |
|  **Target** | Fertilizer Name |





## ⚙️ Installation & Setup

### Prerequisites

Make sure you have the following installed:
- Python 3.8+
- pip
- Git

---

###  Step-by-Step Setup

**1. Clone the Repository**

```bash
git clone https://github.com/your-username/Fertilizer-Prediction-System.git
cd Fertilizer-Prediction-System
```

**2. Create a Virtual Environment**

```bash
# On Windows
python -m venv venv
venv\Scripts\activate

# On macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

**3. Install Dependencies**

```bash
pip install -r requirements.txt
```

**4. Set Up OpenWeather API Key**

> Get your free API key from [OpenWeatherMap](https://openweathermap.org/api) and add it to `App1.py`:

```python
API_KEY = "your_openweather_api_key_here"
```

**5. Run the Flask Application**

```bash
python App1.py
```

**6. Open in Browser**

```
http://127.0.0.1:5000/
```

---

##  Screenshots

<div align="center">

###  Home Page — Input Form
![Home Page](static/images/screenshot_home.png)


---

###  Result Page — Fertilizer Recommendation
![Result Page](static/images/screenshot_result.png)


</div>

---

##  How It Works

```
User Input (N, P, K, Humidity, Moisture, Soil Type, Crop Type)
        ↓
Real-Time Temperature Fetched via OpenWeather API
        ↓
Data Encoded using Pre-trained Label Encoders
        ↓
Naive Bayes Model Predicts Fertilizer
        ↓
Result Displayed on Web Interface 
```

---

##  Requirements

```txt
Flask
scikit-learn
numpy
pandas
requests
pickle-mixin
```

> Install all at once: `pip install -r requirements.txt`

---

##  Contributing

Contributions are welcome! Here's how:

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/YourFeature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/YourFeature`
5. Open a Pull Request 🚀



##  Author

<div align="center">

**Sanika Malwade**

*Data Science & Web Developer*

[![GitHub](https://img.shields.io/badge/GitHub-Sanika--Malwade15-181717?style=for-the-badge&logo=github)](https://github.com/Sanika-Malwade15)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/sanika-malwade)
</div>

---

<div align="center">

###  Built with passion for smart agriculture |  Empowering farmers with AI

*If this project helped you, please consider giving it a ⭐ — it means a lot!*

</div>
