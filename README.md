# Welcome to Heart Disease Predictor

This program uses python for implementation,so please make sure that you ahve the latest version of python installed :)

## Before running the program, please ensure that you have the following libraries installed
` 1. [] Streamlit
  2. [] pandas
  3. [] numpy
  4. [] scikit-learn
  5. [] joblib
  6. [] matplotlib
  7. [] Seaborn`

for any missing library please run the following command in your terminal 
     `pip install <library_name>`

 ** --> To run the program simply run the *run_all.py* file by using the command given below in terminal to execute the code and get to the site**

       python3 run_all.py 
### here is a guide on how the predictor works
firstly)
 A. Train the ML Models (model_training.py)
   
    Load the dataset (heart.csv)

    Split it into training & testing sets

    Train 3 ML models

    Save them using joblib.dump(...) to .pkl files

    So that we don’t have to retrain the model every time the app runs

Secondly)
  B. Create the Streamlit Web App (app.py)
     
    📥 Input Collection
    Users input their health data using sliders/dropdowns in the sidebar (e.g., age, sex, chest pain type, etc.)

    📊 Data Visualization
    Shows a preview of the dataset

    Displays a bar chart of how many patients have heart disease vs. not

    Shows a scatter plot of age vs. max heart rate, colored by target (disease or not)


## How the model looks for the end user 

🧠 Model Selection
User chooses a model (logistic, random forest, or KNN) from a dropdown

📈 Prediction
The app takes the user’s input and passes it into the selected model

The model outputs:

1 → person has heart disease

0 → person does not

The result is displayed using st.success() or st.error() with emojis and colors
