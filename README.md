# Disaster Response Pipeline Project
**Project Motivation:**

In this project. I made use of the data engineering concepts to analyze disaster data from Figure Eight to build a model for an API that classifies disaster messages.

The datasets used contain real messages that were sent during disaster events. 

Our goal here is to build a machine learning model to identify if these messages are related to disaster or not, and further label the nature of these messages. This would be of great help for some disaster relief agencies. We have 36 labels for these messages in total. Note, however, these labels are not mutually exclusive. Hence it is a multi-label classification problem

**Instructions:**
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/


**Requirements**

    Python 3.5+
    NLTK for natural language processing (converting text data into numerical data)
    Pandas, Numpy, scikit-learn, sqlalchemy for data processing and machine learning
    Matplotlib, seaborn, plotly for data visualizations
    Flask, back-end of our minimalistic web app
