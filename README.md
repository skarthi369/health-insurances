# health-insurances

# Medical Insurance Cost Prediction

This project aims to predict medical insurance costs using machine learning. It utilizes a dataset containing information about individuals' age, sex, BMI, smoking habits, region, and number of children to train a regression model. The model can then be used to estimate the insurance expenses for new individuals based on their characteristics.

## Dataset

The dataset used in this project is named `insurance.csv`. It contains the following columns:

- **age:** Age of the individual.
- **sex:** Gender of the individual (male/female).
- **bmi:** Body Mass Index of the individual.
- **children:** Number of children the individual has.
- **smoker:** Whether the individual is a smoker (yes/no).
- **region:** Region where the individual resides (northeast, northwest, southeast, southwest).
- **expenses:** Annual medical expenses of the individual.

## Methodology

1. **Data Loading and Preprocessing:**
   - The dataset is loaded using pandas.
   - Categorical features (sex, smoker, region) are one-hot encoded using OneHotEncoder.
   - Numerical features (age, bmi, children) are scaled using StandardScaler.

2. **Model Training:**
   - The dataset is split into training and testing sets using train_test_split.
   - A Gradient Boosting Regressor model is trained on the training data.

3. **Model Evaluation:**
   - The model's performance is evaluated using metrics such as Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared (R2) score.

4. **Deployment:**
   - The trained model is saved as a pickle file (`gradient_boosting_regressor_model.pkl`).
   - A Flask web application is created to allow users to input their information and get insurance cost predictions.
   - ngrok is used to expose the web application publicly.


## Usage

1. **Clone the repository:**

2. 2. **Install dependencies:**
   3.  pip install -r requirements.txt
  
   4.  3. **Run the Flask application:**
     
       4. 4. **Access the application:**
   - Open the public URL provided by ngrok in your web browser.
   - Enter your information in the input fields.
   - Click the "Predict" button to get your insurance cost prediction.

## Contributing

Contributions to this project are welcome! Please feel free to open issues or pull requests.

## License

This project is licensed under the MIT License.


