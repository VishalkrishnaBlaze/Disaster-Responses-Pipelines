# Disaster Response Pipeline Project

### Description
----
This Project is part of Data Science Nanodegree Program by Udacity in collaboration with Figure Eight. The initial dataset contains pre-labelled tweet and messages from real-life disaster. The aim of the project is to build a Natural Language Processing tool that categorize messages.

The Project is divided in the following Sections:

1. Data Processing, ETL Pipeline to extract data from source, clean data and save them in a proper databse structure
2. Machine Learning Pipeline to train a model able to classify text message in categories
3. Web App to show model results in real time.

### Getting Started
----
#### Dependencies
* Python 3.5+
* Machine Learning Libraries: NumPy, SciPy, Pandas, Sciki-Learn
* Natural Language Process Libraries: NLTK
* SQLlite Database Libraqries: SQLalchemy
* Web App and Data Visualization: Flask, Plotly
#### Installing
Clone this Git repository:
`https://github.com/VishalkrishnaBlaze/Disaster-Responses-Pipelines.git`
#### Execution:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/
#### Results

1. The first page that you get
![First page](Screenshots/intro.png)
----
2. This is an example of a message you can type to test Machine Learning model performance
![Sample Input](screenshots/sample_input.png)
----
3. After clicking **Classify Message**, you can see the categories which the message belongs to highlighted in green
![Sample Output](screenshots/sample_output.png)
----
4. The main page shows some graphs about training dataset, provided by Figure Eight
![Main Page](screenshots/main_page.png)
