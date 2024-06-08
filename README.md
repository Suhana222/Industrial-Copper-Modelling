# Industrial-Copper-Modelling

![Screenshot_8-6-2024_225040_localhost](https://github.com/Suhana222/Industrial-Copper-Modelling/assets/167739067/e56e867f-d4d5-4460-8cf1-75010d52d4c9)

## Overview


The Industrial Copper Modeling Application is a web-based tool built with Streamlit, designed to help users predict the selling price and status of industrial copper products based on various parameters. 
This application leverages machine learning models to provide accurate predictions, enhancing decision-making processes in the copper industry.

##  Technologies Used

The Industrial Copper Modeling Application is built using a combination of several technologies and libraries. Below is a detailed list of the main technologies used:

### Frontend

Streamlit:

1.A powerful, easy-to-use framework for building and deploying data-driven applications.

2.Provides a simple API to create interactive web applications using Python.

### Backend

Python:

A versatile programming language used for developing the core logic of the application.

### Machine Learning

scikit-learn:

1.A robust library for machine learning in Python.

2.Used for loading pre-trained models and performing data preprocessing tasks like scaling and encoding.

### Data Processing

Numpy:

1.A fundamental package for scientific computing with Python.

2.Provides support for arrays and matrices, along with a large library of mathematical functions to operate on these arrays.

Pandas:

1.A powerful, open-source data analysis and manipulation tool built on top of the Python programming language.

2.Used for reading and processing data from various file formats, including Excel.

### Model Serialization

Pickle:

1.A Python module for serializing and deserializing Python object structures.

2.Used to save and load machine learning models and preprocessing objects.

### Regular Expressions

re:

1.A module for working with regular expressions in Python.

2.Utilized for input validation to ensure the correct format of numerical inputs.

### Web Development

HTML/CSS:

1.Utilized within Streamlit to enhance the styling and layout of the application interface.

2.Custom HTML and CSS are embedded within the Streamlit application to provide a polished look and feel.

## Step by Step Procedure

### Installation

To set up and run this application, follow these steps:

### Download Required Files:

Ensure you have the following files in your project directory:

1.app.py: The main application script.

2.model.pkl: Serialized model for predicting the selling price.

3.cmodel.pkl: Serialized model for predicting the status.

4.scaler.pkl, t.pkl, s.pkl, cscaler.pkl, ct.pkl: Scalers and transformers for data preprocessing.

5.Copper_Set.csv: The CSV file containing the data.

### Install Python:

Make sure you have Python installed on your system. 

### Install Required Libraries:

pip install streamlit pandas numpy scikit-learn

### Run the Application:

Launch the Streamlit application using the following command:

streamlit run app.py

This will start the Streamlit server and open the application in your default web browser.

### Usage

Upon running the application, you will see a web interface with two main tabs: PREDICT SELLING PRICE and PREDICT STATUS.

### Predict Selling Price

Navigate to the PREDICT SELLING PRICE tab.

Fill in the Input Fields:

1.Status: Choose from options like 'Won', 'Draft', 'To be approved', etc.

2.Item Type: Select from options like 'W', 'WI', 'S', etc.

3.Country: Pick the corresponding country code from the dropdown.

4.Application: Choose the application code from the dropdown.

5.Product Reference: Select the product reference code.

6.Quantity Tons: Enter the quantity in tons. Make sure to use numeric values.

7.Thickness: Enter the thickness of the product.

8.Width: Enter the width of the product.

9.Customer ID: Input the customer ID.

Submit the Form:

Click the PREDICT SELLING PRICE button to get the prediction.

View the Results:

The predicted selling price will be displayed below the button.

### Predict Status

Navigate to the PREDICT STATUS tab.

Fill in the Input Fields:

1.Quantity Tons: Enter the quantity in tons.

2.Thickness: Enter the thickness of the product.

3.Width: Enter the width of the product.

4.Customer ID: Input the customer ID.

5.Selling Price: Enter the selling price.

6.Item Type: Select from options like 'W', 'WI', 'S', etc.

7.Application: Choose the application code from the dropdown.

8.Product Reference: Select the product reference code.

### Submit the Form:

Click the PREDICT STATUS button to get the prediction.

### View the Results:

The predicted status ("Won" or "Lost") will be displayed below the button.

### Models and Data

Machine Learning Models:

1.model.pkl: Used for predicting the selling price.

2.cmodel.pkl: Used for predicting the status.

### Data Preprocessing:

1.scaler.pkl: Standard scaler for normalizing the data.

2.t.pkl: Transformer for one-hot encoding item types.

3.s.pkl: Transformer for one-hot encoding status.

4.cscaler.pkl: Standard scaler for status prediction data.

5.ct.pkl: Transformer for one-hot encoding item types for status prediction.


## Conclusion

The Industrial Copper Modeling Application is an efficient tool for predicting the selling price and status of copper products, utilizing advanced machine learning models to provide accurate insights.
By following the detailed setup and usage instructions, users can leverage this application to make informed decisions in the copper industry. 
The combination of Streamlit for the frontend, Python for backend processing, and various machine learning libraries ensures a robust and user-friendly experience. This application exemplifies how technology can be harnessed to streamline industrial processes and enhance decision-making capabilities.


