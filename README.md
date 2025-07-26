# Weather-Data-Classification
Predicting Future Humidity Levels Using Machine Learning
🧠 Project Title
Humidity Forecasting at 3PM Based on 9AM Weather Conditions Using Machine Learning
📝 Aim
The ultimate goal of this project is to build a Machine Learning model that can predict the relative humidity at 3PM using atmospheric and weather measurements taken at 9AM. We also evaluate the model's accuracy and effectiveness using metrics such as confusion matrix and classification report.
📁 Dataset
Input File: weather.csv, daily_weather.csv
Target Feature: relative_humidity_3pm
The dataset includes various atmospheric measures recorded at 9AM and 3PM, such as:
Air Pressure
Temperature
Wind Speed & Direction
Rain Accumulation & Duration
Relative Humidity
🧪 Process Flow
1. 📥 Data Loading & Inspection
Loaded weather data using pandas.
Explored dataset structure using .head(), .info(), .describe(), etc.

2. 📊 Descriptive Statistics
Calculated:
Mean, Median, Mode of relative_humidity_3pm.
Range, Variance, Standard Deviation for air_pressure_9am.

3. 🧹 Data Preprocessing
Handled missing values using .dropna() and .fillna(0).
Labeled relative_humidity_3pm:
1 → Humidity > 25\
0 → Humidity ≤ 25

4. 🔍 Outlier Detection & Visualization
Used Box Plots, Scatter Plots, and Q-Q Plots.
Identified outliers using Z-score method.

5. 📈 Exploratory Data Analysis
Univariate Analysis: Histograms, Box plots.
Bivariate Analysis: Scatter plots and Correlation Heatmaps.
Multivariate Analysis: Pairplots.

6. 🎯 Feature Selection
Selected 9AM features (air_pressure_9am, air_temp_9am, rain_duration_9am, etc.) for prediction.

7. 🧠 Model Building
Model Used: DecisionTreeClassifier with entropy criterion.
Train-Test Split: 70-30 ratio using train_test_split.
Scaling: Applied StandardScaler for normalization.

8. 📉 Model Evaluation
Evaluated with:
Confusion Matrix
Accuracy Score
Classification Report (Precision, Recall, F1-Score)

🔧 Tech Stack
Languages: Python
Libraries Used:\
pandas, numpy, matplotlib, seaborn
sklearn for ML model and metrics
scipy for statistical analysis

✅ Results
Model: Decision Tree Classifier
Accuracy: Displayed as percentage (e.g., accuracy_score * 100)
Classification Report: Includes performance metrics for both classes (0 & 1)

📂 Output
A trained Decision Tree Classifier.
Visualization of decision tree using tree.plot_tree().
CSV file with a new column: classified (0 or 1 based on humidity at 3PM).
