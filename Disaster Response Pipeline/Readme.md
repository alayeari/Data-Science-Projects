#### File Descriptions
###### app
- template
- master.html  # main page of web app
- go.html  # classification result page of web app
- run.py  # Flask file that runs app

###### data
- disaster_categories.csv  # data to process 
- disaster_messages.csv  # data to process
- process_data.py
- InsertDatabaseName.db   # database to save clean data to

###### models
- train_classifier.py

#### Components
There are three components I completed for this project.

##### 1.ETL Pipeline
A Python script, process_data.py, writes a data cleaning pipeline that:

- Loads the messages and categories datasets
- Merges the two datasets
- Cleans the data
- Stores it in a SQLite database
- A jupyter notebook ETL Pipeline Preparation was used to do EDA to prepare the process_data.py python script.

##### 2. ML Pipeline
A Python script, train_classifier.py, writes a machine learning pipeline that:

- Loads data from the SQLite database
- Splits the dataset into training and test sets
- Builds a text processing and machine learning pipeline
- Trains and tunes a model using GridSearchCV
- Outputs results on the test set
- Exports the final model as a pickle file
- A jupyter notebook ML Pipeline Preparation was used to do EDA to prepare the train_classifier.py python script.

##### 3. Flask Web App
- The project includes a web app where an emergency worker can input a new message and get classification results in several categories. The web app will also display visualizations of the data. The outputs are shown below:

