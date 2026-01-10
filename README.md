##🏠 VRENTAL Price Predictor
An interactive machine learning tool designed to recommend optimal rental prices for property listings based on location quality, room dimensions, and available amenities.

##🚀 Overview
The VRENTAL Price Predictor bridges the gap between raw machine learning models and end-user utility. By utilizing a trained regression model, this script provides a user-friendly interface to estimate the market value of a rental unit in real-time.

##🛠️ How It Works
The script follows a simple three-step pipeline:
User Input: Collects real-time data via a CLI panel (Location Score, Square Footage, and Amenities).
Data Processing: Formats the input into a pandas DataFrame to match the model's training schema.
Inference: Pass the data through the model.predict() function to output a recommended price in INR.

##📊 Features Used for Prediction
The model calculates the rental price ($y$) based on the following independent variables ($x$):
Location Score: A decimal value (1.0–10.0) representing the desirability and proximity of the area.
Room Size: Total area of the listing in square feet.Amenities Count: The number of perks included (e.g., WiFi, AC, Laundry, Food).

##💻 Installation & Usage
Prerequisites
Ensure you have Python installed along with the following libraries:
Bashpip install pandas scikit-learn
Running the Predictor
Clone this repository.Ensure your trained model object is loaded into your environment.
Run the script:
Pythonpython predictor_script.py
Example Input/Output
Plaintext
--- INTERACTIVE PRICE PREDICTOR ---
Enter Location Score (e.g., 8.5 for Prime): 9.2
Enter Room Size (in sqft, e.g., 260): 300
Enter Amenities Count (e.g., 4): 5

==================================================
**ML Model Recommendation for Input:**
  Location Score:  9.2
  Room Size (sqft):300
  Amenities Count: 5
--------------------------------------------------
  Optimal Predicted Rental Price: **₹18,500**
==================================================
##⚠️ Error Handling

The script includes a try-except block to catch ValueErrors. 
If a user enters text where a number is expected, the system will provide a clean exit message rather than crashing, ensuring a smooth user experience.

