# Starbucks Offer
Capstone Project for Udacity Data Science NanoDegree

### Table of contents
* [Installation](Installation)
* [Project Overview](Project-Overview)
* [File Descriptions](File-Descriptions)
* [Deliveries](Deliveries)
* [Acknowledgements](Acknowledgements)

### Installation
* python 3.6 or later
* all packages specified in the first section of notebooks

### Project Overview

For business stand of points, Starbucks needs to find a way to present each customer the right offers. So the goal of this project is to use the data to identify which groups of people are most responsive to which type of offer, and to predicts how much someone will spend based on demographics and offer type.

### File Descriptions

##### Data
Starbucks provided simulated data that mimics customer behavior on the Starbucks rewards mobile app. There are three datasets:
* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
* profile.json - demographic data for each customer
* transcript.json - records for transactions, offers received, offers viewed, and offers completed Here is the schema and explanation of each variable in the files:

**portfolio.json**
* id (string) - offer id
* offer_type (string) - type of offer ie BOGO, discount, informational
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) -
* channels (list of strings)

**profile.json**
* age (int) - age of the customer
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income

**transcript.json**
* event (str) - record description (ie transaction, offer received, offer viewed, etc.)
* person (str) - customer id
* time (int) - time in hours. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record


##### Notebooks
* Preprocessing_Exploration.ipynb: Data proprocessing, cleaning and dataset exploration
* Modeling.ipynb: models to predict if someone will response to an offer and how much someone will spend.


### Deliveries
Check out [Medium article](https://medium.com/p/4ac9ce83b636/edit) for this project

### Acknowledgements
This project was completed as part of the Udacity Data Science Nanodegree. The datasets used here were provided by Starbucks Coffee Company.
