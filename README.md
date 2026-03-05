This Streamlit App utilizes a Machine Learning API built with FastAPI in order to detect lung cancer in patients based on the following criteria: age, gender, blood pressure, smoke, coughing, allergies, fatigue etc.

​The machine learning model used for this app was deployed as an API using the FastAPI framework and then accessed through a frontend interface with Streamlit.

The data was then cleaned and processed for modelling by changing the following:

The values "M" and "F" in the "GENDER column were converted to 1 and 0 respectively.
The values "YES" and "NO" in the "LUNG_CANCER" column were converted to 1 and 0 respectively.
The values "2" and "1" in the rest of the columns were converted to 1 and 0 respectively.
The processed dataset was then saved as processed_lung_cancer.csv

Modelling
In this project I tested 6 different classification algorithms namely:

Logistic Regression
Decision Tree
Random Forest
XGBoost
GradientBoostClassifier
SupportVectorClassifier
The final model used for the API was the Gradient Boost Classifier model which had an accuracy score of 0.94.

Clone the repository to your local machine
Install docker and docker-compose if you haven't
Open a bash/cmd in the directory and run:
docker network create AIservice
Then run this command
docker-compose up -d --build
After the above steps have been carried out you can now view the documentation of the API and also the Streamlit app.
