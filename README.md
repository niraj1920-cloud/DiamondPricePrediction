
# Diamond Price Prediction using Machine Learning




## About the Project
The Diamond Price Prediction project is an end-to-end machine learning initiative designed to forecast the prices of diamonds. Diamonds are highly valuable gemstones, and their prices can vary significantly based on various factors. This project aims to leverage machine learning techniques to provide accurate predictions of diamond prices, thereby offering valuable insights to both buyers and sellers in the diamond market.
## About Dataset
The goal is to predict price of given diamond (Regression Analysis).

There are 10 independent variables (including id):

- id : unique identifier of each diamond
- carat : Carat (ct.) refers to the unique unit of weight measurement used exclusively to weigh gemstones and diamonds.
- cut : Quality of Diamond Cut
- color : Color of Diamond
- clarity : Diamond clarity is a measure of the purity and rarity of the stone, graded by the visibility of these characteristics under 10-power magnification.
- depth : The depth of diamond is its height (in millimeters) measured from the culet (bottom tip) to the table (flat, top surface)
- table : A diamond's table is the facet which can be seen when the stone is viewed face up.
- x : Diamond X dimension
- y : Diamond Y dimension
- z : Diamond Z dimension

Target variable:
- price: Price of the given Diamond.

Dataset Source Link : https://www.kaggle.com/competitions/playground-series-s3e8/data?select=train.csv
## Tech Stack
- Pandas
- Numpy
- Scikit-Learn
- Seaborn
- Matplotlib
- Flask
- 
## Project Structure
├── artifacts/                    
│   ├── preprocessor.pkl           # Pickle file for data preprocessing
│   ├── model.pkl                  # Pickle file for the trained model
│   ├── raw.csv                    # Raw dataset file
│   ├── train.csv                  # Training dataset file
│   └── test.csv                   # Testing dataset file
│
├── Logs/
│   └── time_format.log            # Log file capturing run logs and timestamps
│
├── notebooks/                     
│   ├── EDA.ipynb                  # Exploratory Data Analysis (EDA) notebook
│   ├── Model-training.ipynb       # Notebook for model training and evaluation
│   └── data/
│       └── gemstone.csv           # Dataset on diamond details used for analysis
│
├── prediction_tries/
│   ├── prediction.py              # Script for making predictions on test data
│   ├── test_data.csv              # Input test data file for predictions
│   └── test_pred.csv              # Predicted values output file (generated after running prediction.py)
│
├── src/                           # Source code directory
│   ├── exception.py               # Custom exception handling module
│   ├── logger.py                  # Logging module for the project
│   ├── utils.py                   # Utility functions used across modules
│   ├── components/                
│       ├── data_ingestion.py      # Code for data ingestion
│       ├── data_transformation.py # Code for data transformation and preprocessing
│       └── model_trainer.py       # Code for model training
│   └── pipelines/
│       ├── prediction_pipeline.py # Code for the model prediction pipeline
│       └── training_pipeline.py   # Code for the model training pipeline
│
├── application.py                 # Main application file for running the web app
│					
└── setup.py                       # Project's metadata and configuration details for installation


## Installation Steps
Follow these steps to install and set up the project directly from the GitHub repository:

1. Clone the Repository

 - Open your terminal or command prompt.
 - Navigate to the directory where you want to install the project.
 - Run the following command to clone the GitHub repository:
   
```bash
  git clone https://github.com/niraj1920-cloud/DiamondPricePrediction.git
```
2. Create a Virtual Environment (Optional but recommended)
```bash
  conda create -p <Environment_Name> python==<python version> -y
```
3. Activate the Virtual Environment
```bash
  conda activate <Environment_Name>/
```
4. Install Dependencies
- Navigate to the project directory:
```bash
  cd [project_directory]
```
 - Run the following command to install project dependencies:
```bash
  pip install -r requirements.txt
```
5. Run the Project
- Start the project by running the appropriate command.
```bash
  python application.py
```
6. Access the Project
```bash
  http://127.0.0.1:5000/
```

## Screenshots

![image](https://github.com/user-attachments/assets/b5756a8f-1aca-4848-b730-3cdda2cad394)

![image](https://github.com/user-attachments/assets/2f8bb925-451a-4032-9767-824083a97284)



