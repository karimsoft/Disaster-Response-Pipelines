# Disaster Response Pipeline Project

#### Introduction

After a disaster, responsible agencies typically receive millions of direct or social media communications just when disaster response organizations are least able to filter and select the most important messages. Often, only one in a thousand messages is relevant for disaster response professionals. Typically, in response to disasters, Different organizations take care of different parts of the problem. One organization takes care of water, another takes care of blocked roads, another takes care of medical supplies.

#### Objectives

This Project is a part of Data Science Nanodegree Program by Udacity in collaboration with Figure Eight. This project aims to develop a computational model based on the Natural Language Processing (NLP) to classify messages and identify needs after a disaster.

#### Description

This Project is a part of Data Science Nanodegree Program by Udacity in collaboration with Figure Eight. The initial dataset contains pre-labelled tweet and messages from real-life disaster. The aim of the project is to build a Natural Language Processing (NLP) tool that categorize disaster messages.

The Project is divided in the following Sections:

    Data Processing, ETL Pipeline to extract data from source, clean data and save them in a proper database structure.
    Machine Learning Pipeline to train a model able to classify text messages into appropriate categories.
    Web App to show model results in real time.

#### Dependencies

    Python 3.5+ (I used Python 3.8)
    Machine Learning libraries: NumPy, SciPy, Pandas, Sciki-Learn
    Natural Language Process libraries: NLTK
    SQLite Database libraries: SQLalchemy
    Web App and Data Visualization: Flask, Plotly

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/

#### Additional Material

In the data and model folder you can find Jupyter notebooks that will help you understand how the model works step by step:

    ETL Preparation Notebook: an implemented ETL pipeline which extracts, transforms, and loads raw dataset into a cleaned dataset.
    ML Pipeline Preparation Notebook: analyzing machine learning models through NLP process to find the final model.
    ML Pipeline Final Notebook: the final machine learning model used for web app.
 
 
#### Project Structure Files 
    app
    | - template
    | |- master.html # main page of web app
    | |- go.html # classification result page of web app
    |- run.py # Flask file that runs app
    data
    |- disaster_categories.csv # data to process
    |- disaster_messages.csv # data to process
    |- process_data.py
    |- MessageCategoriesETL.db # database to save clean data to
    models
    |- train_classifier.py
    |- model.p # saved model
    README.md


