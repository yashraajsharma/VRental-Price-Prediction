# 🏠 VRENTAL: Interactive Price Predictor

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Machine Learning](https://img.shields.io/badge/Focus-Machine%20Learning-orange.svg)](https://scikit-learn.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

An interactive Machine Learning tool that provides data-driven rental price recommendations. This script allows property managers and owners to input room features and receive an instant, "optimal" market price prediction.

---

## 🚀 Project Overview
In the competitive rental market, pricing a room too high leads to vacancies, and pricing too low leads to lost revenue. **VRENTAL** solves this by using a trained regression model to analyze specific room characteristics and suggest the most profitable price point.

### Key Features:
* **Real-time Inference:** Get predictions instantly via a user-friendly CLI.
* **Data Validation:** Built-in error handling to prevent script crashes from invalid inputs.
* **Human-Readable Output:** Results are formatted clearly with currency symbols and organized tables.

---

## 📊 Feature breakdown
The model predicts the rental price based on three critical variables:

| Feature | Description | Range (Example) |
| :--- | :--- | :--- |
| **Location Score** | A quantitative measure of the neighborhood's desirability. | 1.0 (Low) to 10.0 (Prime) |
| **Room Size** | The physical dimensions of the listing in square feet. | 100 - 500 sqft |
| **Amenities Count** | The number of facilities included (WiFi, AC, Food, etc.). | 1 to 5+ |

---

## 🛠️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/vrental-price-predictor.git](https://github.com/your-username/vrental-price-predictor.git)
   cd vrental-price-predictor

2. **Install dependencies:**
   ```bash
   pip install pandas scikit-learn

3. **Ensure the model is loaded:**
   Place your trained model file in the project directory and ensure your script is pointing to it (e.g., joblib.load('model.pkl')).


## 🖥️ Usage Demo
   Run the script in your terminal to start the interactive panel:
   ```bash
   python price_predictor.py


 **Example Workflow:**

--- INTERACTIVE PRICE PREDICTOR ---
Please enter the features for the new VRENTAL listing:
Enter Location Score (e.g., 8.5 for Prime): 9.0
Enter Room Size (in sqft, e.g., 260): 280
Enter Amenities Count (e.g., 4): 5

==================================================
**ML Model Recommendation for Input:**
  Location Score:  9.0
  Room Size (sqft):280
  Amenities Count: 5
--------------------------------------------------
  Optimal Predicted Rental Price: **₹18,500**
==================================================
