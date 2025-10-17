Applied Data Science Capstone Project
Predicting Falcon 9 First Stage Landing Success
Project Overview

This capstone project explores the prediction of successful landings for the Falcon 9 rocket’s first stage, a key factor in SpaceX’s groundbreaking ability to reuse hardware and reduce launch costs. While SpaceX advertises launches at $62 million—far less than the $165 million charged by traditional providers—this cost efficiency hinges on reliably landing and reusing the first stage. By developing predictive models, we aim to better estimate true launch costs and provide insights for organizations competing in the space launch market.

Project Objectives
The project is organized into sequential modules, each building on the last to form a complete end-to-end data science pipeline culminating in predictive modeling. Highlights of each phase are detailed below:

1. Acquiring and Preparing Data from the SpaceX API
Data Collection: Initiated by fetching historical SpaceX launch data through the SpaceX API, capturing vital parameters for analysis.
Data Cleaning: Standardized and cleaned the dataset by addressing inconsistencies, resolving missing values, and shaping the data for downstream use.
2. Web Scraping for Falcon 9 Launch Records
BeautifulSoup Web Scraping: Utilized BeautifulSoup to extract detailed Falcon 9 launch histories from Wikipedia.
Data Parsing and Structuring: Converted scraped HTML tables into Pandas DataFrames for seamless manipulation and further analysis.
3. Exploratory Data Analysis (EDA) and Label Assignment
Visual Exploration: Leveraged visualization libraries such as Matplotlib and Seaborn to uncover patterns, trends, and correlations in the data.
Data Labeling: Developed and assigned target labels for use in supervised machine learning.
4. Database Integration and Querying
Db2 Database Loading: Imported data into an IBM Db2 database to take advantage of SQL’s capabilities for structured querying.
SQL Analysis: Designed and executed custom SQL queries to extract additional insights about launches and outcomes.
5. Feature Engineering and Geospatial Visualization
Feature Creation: Engineered new features from existing data to boost model accuracy and interpretability.
Interactive Mapping: Used Folium to create interactive maps, revealing how launch locations relate to outcomes and uncovering spatial patterns in success/failure rates.
6. Interactive Analytics via Plotly Dash
Dash Application Development: Built an interactive dashboard with Plotly Dash, enabling real-time data exploration.
User Controls: Added dynamic widgets like dropdowns and sliders, allowing users to engage with pie charts and scatter plots for a deeper dive into the data.
7. Machine Learning and Model Refinement
Preprocessing: Standardized and split the dataset into train and test sets for robust model assessment.
Hyperparameter Tuning: Applied GridSearchCV for optimal tuning across model types, including SVM, Decision Trees, and Logistic Regression.
Performance Evaluation: Compared model results to identify the best approach for “landing success” prediction.
Summary of Results
Best Model: The Decision Tree Classifier emerged as top performer, reaching 0.9444 accuracy on the test set.
Other Models: Both Support Vector Machine and K-Nearest Neighbors achieved a respectable 0.8333 accuracy.
Conclusion
Through careful data gathering, cleaning, feature engineering, and comprehensive modeling, this project provides a reliable method to predict Falcon 9 landing success. The resulting insights can help estimate launch costs and inform bidding strategies for companies seeking to challenge SpaceX’s dominance in commercial spaceflight.

Repository Overview
data/: Raw datasets and data management scripts
notebooks/: Jupyter notebooks documenting each stage of the project
scripts/: Python scripts for data prep, analysis, and modeling
dash_app/: Codebase for the Plotly Dash interactive dashboard
README.md: In-depth project summary and instructions
Acknowledgments
Special thanks to IBM for providing resources and to Coursera for hosting the course materials.
