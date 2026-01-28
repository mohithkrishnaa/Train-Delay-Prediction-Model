# Train-Delay-Prediction-Model
Train Delay Prediction using Machine Learning. This project predicts train arrival delay categories (on-time, slight delay, major delay) using real-world railway data. Built with XGBoost, it includes data preprocessing, EDA, class-balanced evaluation, and deployment as an interactive Streamlit web app

🎯 Objectives

Analyze railway schedules and operational patterns influencing delays

Identify key delay-causing factors using Exploratory Data Analysis (EDA)

Build a robust machine learning model for delay category prediction

Evaluate model performance using class-balanced metrics

Deploy the model as an interactive web application

📊 Dataset

Type: Real-world railway operational data

Size: 250,000+ records

Granularity: Service-level and stop-level information

Key Features:

Train number, service type, operator

Station code, platform, stop order

Arrival hour, day of week, month, weekend flag

Previous stop delay and maximum historical delay

Target Variable (Multi-class):

On-time (0–2 minutes)

Slight delay (2–5 minutes)

Major delay (>5 minutes)

🛠️ Data Preprocessing

Removed cancelled and incomplete records

Handled missing values and data inconsistencies

Encoded categorical variables

Engineered time-based features

Addressed class imbalance using class weighting

🔍 Exploratory Data Analysis (EDA)

Key insights:

Strong correlation between arrival and departure delays

Delay propagation across consecutive stops

Highly right-skewed delay distribution

Majority of trains arrive on time

Conclusion:
A classification-based approach is more robust than regression for this problem.

🤖 Model & Methodology

Approach: Supervised Machine Learning

Problem Type: Multi-class classification

Algorithm Used: XGBoost Classifier

Handles non-linear patterns efficiently

Performs well on tabular data

Robust to outliers and class imbalance

📈 Model Evaluation

Metrics Used:

Precision

Recall

F1-Score

Balanced Accuracy

Accuracy alone was avoided due to class imbalance; balanced metrics provide a fair evaluation across all delay categories.

🌐 Deployment

Deployed as an interactive Streamlit web application

Users input train and arrival details

Outputs:

Predicted delay category

Probability distribution for each class

Results:

High reliability for on-time predictions

Improved recall for delayed classes

Acceptable overall model performance

🔮 Future Scope

Integrate weather and traffic data

Use sequential models to capture delay propagation

Increase historical data depth

Improve class balance further

✅ Conclusion

This project demonstrates an end-to-end machine learning pipeline, from data preprocessing and modeling to deployment. It showcases real-world applicability of ML in transportation analytics and provides hands-on experience in building and deploying scalable ML solutions.
