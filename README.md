**Turbofan Engine Remaining Useful Life (RUL) Prediction**\n
This project focuses on predicting the Remaining Useful Life (RUL) of turbofan engines using machine learning and deep learning techniques. The goal is to build accurate predictive models that can estimate how many operational cycles an engine has left before it is likely to fail. This is a critical task in predictive maintenance, helping to prevent catastrophic failures and optimize maintenance schedules.

The project uses the NASA Turbofan Engine Degradation Simulation dataset, which provides time-series data from multiple sensors on a fleet of engines.

**Project Notebooks**
This repository contains a series of Jupyter notebooks that walk through the entire process of data handling, feature engineering, and model development:

* file_creation.ipynb: This notebook processes the raw text files from the NASA dataset. It cleans the data, calculates the RUL for each engine, and saves the processed data into CSV files, which are easier to work with.

* Feature_selection.ipynb: Here, we perform an in-depth analysis of the sensor data to select the most relevant features for predicting RUL. This helps to reduce noise and improve model performance.

* Training_Model_with_processed_data.ipynb: This notebook uses the selected features to train a Random Forest Regressor. It evaluates the model's performance on both the training and testing datasets to ensure its accuracy.

* Trial_CNN_with_function_Explained.ipynb: In this notebook, we explore a more advanced approach using a Convolutional Neural Network (CNN). The time-series data is formatted into a sequence that the CNN can process, offering a different perspective on prediction.

**Methodology**
The project follows a structured approach to solving the RUL prediction problem:

* Data Preprocessing: The initial step involves cleaning the raw data, assigning proper column names, and calculating the RUL for each engine cycle. This creates a clean, labeled dataset ready for modeling.

* Feature Engineering: We analyze the sensor measurements to identify which ones are most indicative of engine wear and tear. By selecting the most informative features, we can build more robust and efficient models.

**Model Training:**

* A Random Forest Regressor is trained on the processed data. This model is excellent for handling complex, non-linear relationships in the data.

* A Convolutional Neural Network (CNN) is also implemented to capture temporal patterns in the sensor data, treating the problem as a sequence analysis task.

**Evaluation:** The models are evaluated using the Root Mean Squared Error (RMSE) to measure their predictive accuracy.

**Results**
The project successfully demonstrates two different approaches to RUL prediction:

* The Random Forest Regressor provides a strong baseline performance, effectively capturing the relationships between sensor readings and engine health.

* The CNN model offers a deep learning-based solution that can identify complex temporal features, showing promise for further improvement.

The performance of each model is detailed in its respective notebook, with visualizations to help interpret the results.

Contributing
Contributions are welcome! If you have any ideas for improvements or find any issues, feel free to open an issue or submit a pull request.
