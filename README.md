# DSC412-project

https://colab.research.google.com/drive/1yz2okCCAB-7cDR3qEtmNMaMEaYUi8pLm?usp=sharing

https://drive.google.com/file/d/16PntwaI3jwRmviTchVRBs0w1HnKQWoZu/view?usp=sharing

Thanks for being interested in this StockPrediction project! This project attempts to build a model to predict the price of Apple Inc. (AAPL). 

SUMMARY:

Here is a brief summary of the project:
1. Import Libraries
2. Load and Read an Initial CSV File with Apple's (AAPL) Stock Data

This steps involves the bulk of data preprocessing, data cleansing, and removal of NaN values.

3. Calculate Additional Features

Since the end goal is to build a working ML model, feature engineering is key to doing so. This step calculates some other metrics which helps with model accuracy.

4. Exploratory Data Analysis

Exploring trends between different variables and different metrics helps with fine-tuning the model and understanding which ones are closely related.

5. Train Test Split and Basic Models

This performs the train-test split on the initial data. Some basic models are built as a baseline for loss including Linear Regression, Random Forest, and SVR since they prove to be useful with Time Series data based on some preliminary research.

6. Building, Training, and Saving the Model

This step builds the LSTM model. After training the model, it is saved to avoid having to re-train the model every time you run the file. The loss or cost at the end is 0.0011 which is excellent.

7. Running the Model to Predict Price on the Testing Data

This step is the culminating step, allowing us to see the model in action, comparing actual prices with the predicted prices.

HOW TO RUN THIS PROJECT:

If running the file in Google Colab, upload the AAPL_historical_data.csv file with some preliminary data and the stock_prediction_lstm_aapl.h5 file which contains the TensorFlow model to be run. Then, Google Colab should allow you to run each cell until you are able to get the appropriate output. PLEASE NOTE: Google Colab files are NOT saved! You must manually upload input files and download output files to prevent losing data!

If running the file in VS Code, activate the virtual environment and run requirements.txt to install the necessary libraries/packages by running:

pip install -r requirements

Then, ensure that both of the files mentioned above are in your project directory. Once all of the requirements are installed, you should be able to run each cell until you get the appropriate output.