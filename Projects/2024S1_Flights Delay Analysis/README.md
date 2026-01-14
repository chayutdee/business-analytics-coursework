# Flights Delay Analysis - Portfolio Part 4

## Project Overview 
This project analyzes flight delay data from the U.S. Department of Transportation's (DOT) Bureau of Transportation Statistics (BTS) for 2008. The dataset includes detailed information on domestic flights operated by major U.S. air carriers, focusing on on-time performance, delays, cancellations, and diversions. The main goals of this analysis are:

1) Predicting arrival delay times based on departure-related features using a linear regression model.
2) Predicting flight status (on-time, delayed, canceled, or diverted) using classification models like K-Nearest Neighbors (KNN) and Multilayer Perceptron (MLP).

## Dataset Description 

The dataset contains a **5% random sample** of the original dataset, totaling 96,838 records. Key features in the dataset include:

- Flight Information: Departure and arrival times, carrier, distance, etc.
- Delay Reasons: Carrier, weather, National Airspace System (NAS), and security delays.
- Flight Status: On-time, slightly delayed, highly delayed, canceled, or diverted.

## Data Preprocessing

- Missing values were handled by filling delays and time features with zeros when flights were canceled or diverted.
- Time features were converted into minutes since the start of the day for consistency in analysis.
- Categorical features, such as carrier codes and cancellation reasons, were encoded to enable use in machine learning models.

## Exploratory Data Analysis (EDA)
Key insights from the EDA include:

- Delay Patterns: Most flights (62.8%) were delayed, with only 36.7% of flights being on time.
- Seasonal Trends: Delays were most severe in June and December, likely due to peak travel seasons.
- Low Cancellation Rates: Only 39 flights were canceled, and 378 were diverted.

## Machine Learning Models
1. Linear Regression for Arrival Delay Prediction
- Model: Ordinary Least Squares (OLS) regression.
- Features: Departure-related data (e.g., scheduled departure time, taxi-out time).
- Performance: R-squared = 0.9471, indicating that the model explains 94.71% of the variance in arrival delay times.

2. K-Nearest Neighbors (KNN) for Flight Status Prediction
- Model: KNN classifier.
- Features: Same as those used for delay prediction.
- Performance: Accuracy = 71.74%, F1-Score = 0.6883.

3. Multilayer Perceptron (MLP) for Flight Status Prediction
- Model: Neural network (MLPClassifier).
- Performance: Accuracy = 80.45%, F1-Score = 0.7955. The MLP outperformed the KNN classifier in predicting flight status.

## Conclusion
The analysis demonstrates that departure-related features are strong predictors of arrival delay times. While the MLP classifier improved upon the KNN model, both models were limited by the lack of critical external factors (e.g., weather data) that are crucial for predicting cancellations and diversions.


## Files in the Repository

- 46800883-Portfolio4.py: Script for the project
- DelayedFlights.csv: Sampled dataset of Airline delays
- Reflective Report.md: 
- README.md: This file, providing an overview of the project and instructions.

## Installation 
To run this project, you will need Python and the following Python libraries installed:
- NumPy
- Pandas
- scikit-learn
- Matplotlib
- Seaborn

## Usage 

To replicate the analysis and models in this project:
1. Clone this repository.
2. Navigate to the repository directory and run the Python scripts or Jupyter notebooks.

## Contributing

Warmly welcome contributions from the community and are excited to see your interest in making our project better. Whether you're fixing bugs, adding new features, or improving the documentation, your help is greatly appreciated.
- Incorporate additional features like weather conditions and maintenance records to improve the prediction of cancellations and diversions.
- Experiment with other classification algorithms, such as decision trees or random forests, to enhance accuracy.


## Contact Your Name - chayut.deekongsieng@students.mq.edu.au



```python

```
