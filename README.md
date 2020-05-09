# Disaster-Response-1
This project is to classify disaster response messages through machine learning. 
## Content
- Data
  - disaster_categories.csv and disaster_messages.csv (dataset) thes tow dataset we are using in this project
  - process_data.py: reads in the data, cleans and stores it in a SQL database. Basic usage is python process_data.py MESSAGES_DATA CATEGORIES_DATA NAME_FOR_DATABASE
  - DisasterResponse.db: created database from transformed and cleaned data.
- Models
  - train_classifier.py: includes the code necessary to load data, transform it using natural language processing, run a machine learning model using GridSearchCV and train it. Basic usage is python train_classifier.py DATABASE_DIRECTORY SAVENAME_FOR_MODEL  
- App
  - run.py: Flask app and the user interface used to predict results and display them.
  - templates: This folder contain all the html files required in this project.

## How to run this in the IDE.Following are the command to run the project.
#First u have to go inside the data folder and run the below command.

> python process_data.py disaster_messages.csv disaster_categories.csv DisasterResponse.db

#Secondly you have to go inside the models folder and run the below command

> python train_classifier.py ../data/DisasterResponse.db classifier.pkl

#Lastly move to the app folder and run the below command.

> python run.py
#Screenshot
##First page
![idis](https://user-images.githubusercontent.com/31299019/81468932-0634cb80-9200-11ea-9500-e66cde26d76d.png)

