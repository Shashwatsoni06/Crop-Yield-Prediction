
<img width="2834" height="1282" alt="Screenshot 2025-09-02 022253" src="https://github.com/user-attachments/assets/d6c63f7e-5d17-4e94-85e4-0cec74ae9635" />
<img width="2821" height="1531" alt="Screenshot 2025-09-02 022315" src="https://github.com/user-attachments/assets/b22f5e4b-eebe-46ea-b46d-af2458a7da0e" />
<img width="2836" height="1514" alt="Screenshot 2025-09-02 022329" src="https://github.com/user-attachments/assets/5e6c414a-dfc4-4431-9eb1-094f52680ae0" />
<img width="2844" height="1490" alt="Screenshot 2025-09-02 022345" src="https://github.com/user-attachments/assets/2a1aa54e-3048-4611-86b2-77ee01cc9242" />




Machine Learning Crop Yield Prediction
📖 Overview
This project presents a machine learning approach to predict agricultural crop yield. Using a dataset that combines crop production information with environmental factors like average rainfall and temperature, we've built a model to forecast yield in 'hectograms per hectare' (hg/ha).

The entire workflow, from data exploration and preprocessing to model training and evaluation, is documented in the accompanying Jupyter Notebook. This repository serves as a practical example of applying data science techniques to solve real-world agricultural challenges.

📊 Dataset
The core of this project is the yield_df.csv dataset, which contains historical data on crop production and environmental factors from around the world.

Key features include:

Area: The country where the data was recorded.

Item: The specific crop type (e.g., Maize, Potatoes, Wheat).

Year: The year of the harvest.

average_rain_fall_mm_per_year: The average annual rainfall in millimeters.

pesticides_tonnes: The amount of pesticides used in tonnes.

avg_temp: The average annual temperature in degrees Celsius.

hg/ha_yield: The crop yield in hectograms per hectare (this is our target variable).

🚀 Getting Started
To get a local copy up and running, follow these simple steps.

Prerequisites
Make sure you have Python (3.7+) and pip installed on your system.

Installation
Clone the repository:

git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git)

Navigate into the project directory:

cd YOUR_REPOSITORY

Install the required Python libraries:

pip install pandas numpy matplotlib seaborn scikit-learn jupyterlab

Running the Project
Start Jupyter Lab:

jupyter lab

Open the Untitled2.ipynb notebook from the file browser.

Run the cells sequentially to see the complete analysis and model training process.

🔧 Project Workflow
The project follows a standard machine learning pipeline:

Data Loading & Initial Exploration: The yield_df.csv dataset is loaded into a pandas DataFrame, and an initial assessment of its structure and content is performed.

Data Preprocessing: The dataset is cleaned by handling categorical variables. Features like 'Area' and 'Item' are converted into numerical format using encoding techniques to make them suitable for the model.

Exploratory Data Analysis (EDA): We dive deep into the data to uncover trends, patterns, and correlations between different features and the target variable (yield). Visualizations are used to understand the distribution of data across different countries and crops.

Model Training:

The dataset is split into features (X) and the target variable (y).

It's then further divided into training and testing sets.

A Random Forest Regressor is trained on the training data. This model was chosen for its high accuracy and ability to handle non-linear relationships.

Prediction: The trained model is used to make predictions on new, unseen data points.

📈 Results & Evaluation
The model's performance is a key indicator of its success. Based on the analysis, the model can predict crop yield with a high degree of accuracy.

For instance, given the following input:

Year: 2013

Average Rainfall: 59.0 mm/year

Pesticides: 3024.11 tonnes

Average Temperature: 26.55 °C

Area: Saudi Arabia

Item: Sorghum

The model predicts a yield of 13384.0 hg/ha.

💡 Future Enhancements
This project lays a solid foundation, but there are several avenues for improvement:

Hyperparameter Tuning: Optimize the Random Forest model's parameters to potentially boost its predictive accuracy.

Try Different Models: Experiment with other regression algorithms like Gradient Boosting, XGBoost, or even neural networks.

Expand the Dataset: Incorporate additional features like soil type, fertilizer usage, and irrigation data for a more holistic model.

Deployment: Deploy the trained model as a web application or an API to make it easily accessible for real-time predictions.
