Flight Delay Prediction using LSTM & XGBoost

Overview

This project implements a flight delay prediction system using a hybrid approach combining Long Short-Term Memory (LSTM) networks and XGBoost. The model leverages sequential data processing with LSTM and robust feature selection with XGBoost to achieve an accuracy of 98.40%. The dataset includes various flight parameters such as weather conditions, airline company, and aircraft manufacture year, significantly enhancing prediction performance.

Features

Hybrid Model: LSTM for time-series dependencies & XGBoost for feature selection.

High Accuracy: 98.40% accuracy with Sigmoid activation.

Feature Engineering: Incorporates features like Airline Company and Aircraft Manufacture Year.

Data-Driven Approach: Uses real-world flight delay datasets from US Bureau of Transportation Statistics.

Scalability: Can be applied across different routes and airlines.

Dataset

The dataset is sourced from the US Department of Transport and includes:

Scheduled & Actual Departure/Arrival Times

Carrier Information

Flight Numbers, Origin, and Destination

Weather Conditions

Historical Delays

Dataset Link: Flight Delay & Cancellation Dataset (2019-2023)

Methodology

Data Collection & Preprocessing:

Handling missing values & irrelevant attributes.

Feature engineering (Weather, Airline, Distance, etc.).

Normalization (Min-Max scaling/Z-score normalization).

Model Development:

LSTM Model: Captures sequential patterns.

XGBoost Model: Enhances feature selection and predictive accuracy.

Ensemble Learning: Combining predictions from both models.

Model Evaluation:

Metrics: Accuracy, Precision, Recall, F1 Score.

Cross-validation techniques: 5-fold to 20-fold validation.

Deployment:

Model deployed using Flask/FastAPI for real-time predictions.

User Interface: Allows users to input flight details and receive delay predictions.

Results

Highest Accuracy: 98.40% (Sigmoid Activation)

Best Feature Combination: Airline Company + Aircraft Manufacture Year (98.75% accuracy)

Best Cross-Validation Setting: 20-Fold (98.39% accuracy)

Installation

Clone the repository:

git clone https://github.com/your-repo/Flight-Delay-Prediction.git
cd Flight-Delay-Prediction

Install dependencies:

pip install -r requirements.txt

Run the model training script:

python train.py

Start the Flask API for predictions:

python app.py

Access the web interface at http://localhost:5000.

Technologies Used

Python (Pandas, NumPy, Scikit-learn, TensorFlow, XGBoost)

Deep Learning (LSTM)

Machine Learning (XGBoost, Ensemble Learning)

API Deployment (Flask/FastAPI)

Data Visualization (Matplotlib, Seaborn)

Contributors

Palnika Chavan

Harsha Peshave

Yashraj Panhalkar

Priyanka Shahane (Advisor)

License

This project is licensed under the MIT License.

References

Refer to the research paper for detailed methodology and literature review.

For any inquiries, please contact yashrajpanhalkar146@gmail.com.

