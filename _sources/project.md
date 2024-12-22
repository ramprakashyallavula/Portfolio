## EAS-503-Ecommerce Sales Prediction Project


##  Steps Involved:

### 1 Data Selection and Acquisition
The dataset consisted of historical ecommerce data with features like product categories, prices, revenue, and quantities sold. Data was sourced from structured databases and integrated using SQL queries to retrieve data from normalized (3NF) databases.

---

### 2 Data Preparation and Exploration
Data preparation involved combining relevant tables (e.g., Sales, Product, and Customer tables) using SQL joins. Missing values were handled appropriately, and feature distributions were analyzed to identify patterns and outliers. Relationships between features and target variables were explored through visualizations. Categorical variables were encoded, and numerical features were standardized for consistency.

---

### 3 Machine Learning Experimentation
Reusable pipelines were created to streamline experimentation. Logistic Regression was used as a baseline model, while Random Forest achieved the best performance. Features were engineered to improve accuracy, and dimensionality reduction techniques like PCA were applied to remove noise. Interaction terms were generated to augment the feature space, and impactful features were retained through selection. Model metrics were logged and tracked using MLflow, with Random Forest emerging as the final model based on accuracy, precision, recall, and F1-score.

---

### 4 Model Deployment
The Random Forest model pipeline was deployed as a FastAPI application hosted on Render. A Streamlit web application provided an intuitive interface for users, connected to the FastAPI endpoint for real-time predictions.

---

### 5 Tools and Technologies Used
The project utilized Python for data handling and machine learning, with libraries like Pandas and NumPy for preprocessing. Scikit-learn was used for modeling, while MLflow integrated with DagsHub facilitated experiment tracking and visualization. For deployment, FastAPI and Streamlit were employed to create a functional API and web application, hosted on Render for accessibility. Data visualizations were created using Matplotlib and Seaborn.

---

### 6 Project Outcomes
A robust machine learning pipeline was developed for ecommerce sales prediction. The deployed system provides real-time predictions through an interactive web interface, enabling better business decision-making.

---

### 7 Files and Artifacts

The project comprises several key components that showcase the complete workflow:

- **Notebook:** This Jupyter Notebook documents the entire process, including exploratory data analysis (EDA), feature engineering, and machine learning experimentation, providing a comprehensive view of the project's development.

- **API:** Implemented using FastAPI, this component serves as the backend for deploying the trained model, enabling efficient and scalable prediction services.

- **Web App:** A user-friendly interface built with Streamlit that interacts with the deployed API, allowing users to input data and obtain real-time sales predictions seamlessly.

- **Database:** A structured SQLite database that stores and retrieves cleaned and processed data, ensuring a reliable and consistent data pipeline for analysis and modeling.


### Links Used

- **MLFlow/DagsHub Experiments**: [View Experiments](https://dagshub.com/ramprakashyallavula/Ecommerec/experiments)
- **Docker Hub Repository**: [View Container](https://hub.docker.com/repository/docker/ramprakashyallavula/fastapi-model/general)
- **Deployed Model**: [Deployed FastAPI Model](https://e-commerce-517y.onrender.com/docs)
- **Streamlit App**: [Deployed Streamlit App](https://streamlitt.onrender.com)