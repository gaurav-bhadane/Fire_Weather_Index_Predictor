# Fire Weather Index Predictor

## Overview
This project aims to predict the Fire Weather Index (FWI) using ridge regression on the Algerian forest fire dataset. The FWI is a numerical rating of fire intensity potential, representing the difficulty of controlling fires. The project utilizes Flask for building the web application.

## Dataset
The Algerian Forest Fire Dataset contains meteorological data and fire occurrences for two regions in Algeria (Bejaia region and Sidi Bel-Abbes region) over a period from June 2012 to September 2012. The dataset includes the following columns:

1. **Date**: Date of observation
2. **Temperature**: Temperature in Celsius degrees
3. **RH**: Relative Humidity in percentage
4. **Ws**: Wind speed in km/h
5. **Rain**: Total day in mm
6. **FFMC**: Fine Fuel Moisture Code
7. **DMC**: Duff Moisture Code
8. **DC**: Drought Code
9. **ISI**: Initial Spread Index
10. **BUI**: Buildup Index
11. **FWI**: Fire Weather Index
12. **Classes**: Fire occurrence (Yes/No)

## Requirements
- Python 3
- Flask
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

## Installation
1. Clone the repository: `git clone https://github.com/gaurav-bhadane/Fire_Weather_Index_Predictor.git`
2. 2. Install dependencies: `pip install -r requirements.txt`

## Model Training and Evaluation
The model is trained using Ridge Regression, a type of linear regression that includes L2 regularization to prevent overfitting. The steps for model training and evaluation are as follows:

1. **Data Preprocessing**: 
    - Handle missing values
    - Encode categorical variables
    - Normalize/standardize numerical features

2. **Feature Selection**:
    - Select relevant features based on domain knowledge and exploratory data analysis

3. **Model Training**:
    - Split the dataset into training and testing sets
    - Train the Ridge Regression model on the training set

4. **Model Evaluation**:
    - Evaluate the model on the testing set using metrics like Mean Squared Error (MSE) and R-squared.

## Usage
1. Navigate to the project directory.
2. Run the Flask application: `python application.py`
3. Open a web browser and go to `http://localhost:5000` to access the application.
4. Enter the required weather parameters to predict the FWI.

## Files
- `application.py`: Main Flask application file.
- `templates/`: HTML templates for the web application.
- `data/`: Contains the Algerian forest fire dataset.

## Acknowledgements
- Algerian forest fire dataset: [Link](https://archive.ics.uci.edu/dataset/547/algerian+forest+fires+dataset)
- Flask: [Link](https://flask.palletsprojects.com/)
- Scikit-learn: [Link](https://scikit-learn.org/)

## Contribution
Contributions to the project are welcome. To contribute:

1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature-branch`)
6. Create a new Pull Request
