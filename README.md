
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

![App Screenshot](https://ci3.googleusercontent.com/mail-img-att/AGAZnRrBLeaIny5807rXY__35l1dg3XuzvLk-sNheRTTvsnDF_FVP7QfCzE02EWHbN-DZXyS7ieywSasU2cR3ofrQPAhID4HDCGgCY0EuDLt1M6TcjSVBg5eOZivkyeHNHQLp6r_CZL0xtTZH4iItr88tvfynPnTuBMc85tVPGDNG1PRKMAj35ELvYzKJD8cjdv5v1ICngXNiUwlIJiyzyLQSnS9_Wo9nDyMrKHHASz5l3m53BTGT2w17ubnKaxEaB4RoIhWyseCfJXkjignHTTWFM3q7DrvAK81P1F6c2ONQTiafKvgvlfi8MsxXnEomMT3XvdD44bqvjyN-X5IZxBZ3ru9vzUvv5yCwJgcbA6XUaok9f17Q75OL60QErcjISMj3SLZ00UOYVQKCavQ1Y5YsRZNiiLZqfIgpROtitRzX5dQfugkMqLO5qqU4Gc7wETZW5bX1oXkepLv0C5j6yRlWkK_yVIqslSJQ3iERRd9bQuB2dWD_c64ia8ij0fcFOvppeTZmtxB4vw0JmEKKlzs8bY-MQ-isHqjX8UOHD4Y5sCvXet00jo3Ky6gZkJS85Hfx9L_XupLG1JVLJgp3Piidq9adkgALaNIqRRHOSI7hJnWQrIMtWuh-kLSum3FhsDu-xmADVzr3xSoItnwdIymbdXPQa7FGG9lu5PAPuRmtdGFSC-rSdeyD3B5Fkx_yTVmRlWrJ-x-pghyTeRYXQzhVy2xyXHc62mxrdEWQ_WnzB6h7WZO_FCBRx1gVUXtrlvQqazMgMicH0-gAL_ZpFYmEglf1R2CCld4h24mWnaY2U1jJy5N32-wnCk6nbWPjHcvKiNP_PluL5m3Y2fJ6rndf0YVL3xiYb53lHEHxnkcyCaQirw-aqmCl4f_FgmNNebu9Yxsx3KmJDPbVHs0FfJZ2cN4bpo0-ysPL9NH1MiO-mQ7pF6s_p78CVLUe974sm-219vYNLPWLA34x7sACEsI7LnrcpDa6oy7_Em_jwXpaovcNkUd7CrHBwMFAbea0uVQ4KcmWHk0D-wwCw6v7SnNQzYR0Q=s0-l75-ft)

![App Screenshot](https://ci3.googleusercontent.com/mail-img-att/AGAZnRr66R2FMQ5A68-73D25bIDmoUzbEYVqM1DUcMbBbNcFDGdD5vSZNcBqecgl-9zcAfGKo68MG7enBBoeQwTHedbpE00uRedccporpUObaCuA0SecNEHaXem8IyR9LWz3gv9Ht-AjAFvI3ZDCYRM59LUpI6AjWbFM9Nhmh0fySQ67TakIb6u188LfNBZEpYAiLu5m9hFGuPBHgHxCl_ONrqQS8sNwAR6uYlq03AOr482kOU6PN8MjRXX-AWNcJ9PgUS42hI-i_e_lIZzgAyuAg2IX3Xi0u6t11rirGyyCMud_M3kBjGj-F-It53I19fagskQNKcRE4BTGSaBO-wix5HxpOX4SESiKgkKA83sQ0_XpO2bpUzOhiujXm9xTnIBPZjRh2tLWmLE_TPYabCOy1HuTwcSMfn08842zvofo2k__bWm9-rNbtHLkoGr1uLiCqHKeKsRE6silCLvMSNFqs3EXJCpy8_kGUK-tb5jwt5lTWb_4exDVQRvI3zeS691dzeqTETYpcmcvKxQdWdKreMxn24lgsCBHasv6vljCFirv-EijLk571AiJ6FOxEarQclqL7KRYI8v3N6VwsCNzTDoQbjz9s5wUhEXEK-ycMtxUL1OihEvPeqiIMQPHGRrNYLUUc31oolSoHL0of6SAZAwPYlDS3ewuMFxEfRq3DG64GTwzlIewAaoSsifQBBVH2OyI2mdxrElcaJIZ2Qug6JYnk7AAN-d_f1NSqFbxU0q20WUjOBAbKW0qif1gVPW4NRopg7MC7M5y5izO0TdJQo59bAQrLLxpCr8P9FFohujmJHWelNyqlgrwxoA7eBgTJo4wUtL_rzV3UrWq2MGXbHu1npxJmYSpG7GB9TNLEGtwQg6iF4tcrbIhTen9Gwsrdage0ctJ6M_mSDyXw4OUGFq269pozQrQ0HpeKmK1syMfWO70SUt-5C3iSGZ5buxejIZ76KEruRiOIhBzofHdDdMl9eBdOo3cothPnFjTpsZ9RBiX3QmMHS1uGeFgeOjVv3t_Qfqie_zmmGTZ4hoIfAhvvA=s0-l75-ft)



