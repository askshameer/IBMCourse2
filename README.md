# Applied Data Science Capstone Project

## Predicting Falcon 9 First Stage Landing Success

Welcome to the Applied Data Science Capstone Project! In this project, we develop predictive models to forecast the successful landing of the Falcon 9 rocket’s first stage—a key achievement in SpaceX’s mission to make space travel more cost-effective.

SpaceX advertises Falcon 9 launches at $62 million, compared to the $165 million charged by other providers. This cost difference largely depends on the ability to routinely land and reuse rockets. Accurately predicting the likelihood of a successful landing not only refines launch cost estimates but also equips companies bidding for launches with valuable insights.

---

## Table of Contents

- [Project Objectives](#project-objectives)
- [Workflow & Methodology](#workflow--methodology)
- [Results](#results)
- [Repository Structure](#repository-structure)
- [Getting Started](#getting-started)
- [Acknowledgments](#acknowledgments)

---

## Project Objectives

This project guides users through a complete data science workflow:

- Acquire and prepare launch data from the official SpaceX API and Wikipedia
- Perform exploratory data analysis (EDA) and feature engineering
- Store and query data within a Db2 database environment
- Develop visualizations, including interactive dashboards and geospatial maps
- Build, tune, and evaluate machine learning models to predict launch success

---

## Workflow & Methodology

### 1. Data Acquisition & Preparation

- **SpaceX API Request:** Gathered historical launch data via the SpaceX API—collecting details such as mission dates, payloads, and outcomes.
- **Web Scraping:** Used BeautifulSoup to extract comprehensive Falcon 9 records from Wikipedia.
- **Data Cleaning:** Addressed missing values, standardized formats, and structured the dataset in Pandas.

### 2. Exploratory Data Analysis (EDA) & Labeling

- Visualized data with Matplotlib and Seaborn to identify trends and relationships
- Defined and assigned target labels indicating landing success/failure for supervised learning tasks

### 3. Database Integration

- Uploaded datasets to IBM Db2 for enhanced analysis
- Crafted and performed SQL queries to extract actionable insights

### 4. Feature Engineering & Visualization

- Engineered new features (e.g., payload mass categories, boosters used, launch sites)
- Created interactive maps using Folium to analyze geographical influences on landing outcomes

### 5. Interactive Visual Analytics

- Developed a Plotly Dash application featuring:
    - Dropdowns and sliders for dynamic filtering
    - Real-time interactive pie charts and scatter plots

### 6. Machine Learning Pipeline

- Standardized & split data into train/test sets
- Modeled with Decision Trees, SVM, KNN, and Logistic Regression
- Tuned parameters with GridSearchCV to optimize model performance
- Evaluated and compared results to select the best-performing approach

---

## Results

- **Decision Tree Classifier:** Achieved the best test accuracy (0.9444)
- **SVM & KNN:** Both attained solid accuracy (0.8333)
- **Outcome:** The developed model can reliably estimate the probability of a successful Falcon 9 landing, empowering more informed cost projections and competitive bidding strategies.

---

## Repository Structure
data/ # Raw and processed datasets, data-wrangling scripts
notebooks/ # Jupyter notebooks detailing each module step by step
scripts/ # Python scripts for processing, visualization, and modeling
dash_app/ # Source code for the interactive Plotly Dash dashboard
README.md # This project overview and instructions
---

## Getting Started

1. **Clone the repository:**
2. git clone https://github.com/your-username/falcon9-landing-prediction.git
cd falcon9-landing-prediction
2. **Set up your environment:**  
- Install dependencies from `requirements.txt`
- Configure database credentials (for Db2 module)
- Explore and run the notebooks in sequence

3. **Launch the dashboard:**
cd dash_app
python app.py

Open your browser to view the interactive dashboard.

---

## Acknowledgments

- **IBM**: For providing the course structure and resources
- **Coursera**: For hosting the learning platform and materials

---

Explore the repository to discover the complete data science pipeline—from raw data to interactive dashboards and predictive modeling. Whether your interest lies in data science, space technology, or machine learning, you’ll find actionable techniques and insights within this project.

---
