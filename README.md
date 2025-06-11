


# 🧮 SalarySense: Data Science

A tool to estimate data science salaries (MAE \~ \$11K) to help job seekers negotiate better offers.
Built using data scraped from Glassdoor with Python and Selenium.

---
## 🚀 Project Overview

Upon completing Andrew Ng’s **Machine Learning** course on Coursera and enhancing my skills through hands-on practice on **Kaggle**,by actively engaging in various ML courses and exercises. I initiated this project to deepen my understanding and practical application of machine learning concepts. It proved to be an enriching and intellectually rewarding experience, and it was a genuine pleasure to work on.

* Scraped 1000+ job listings from Glassdoor.
* Extracted and engineered features from job descriptions to evaluate demand for skills (Python, Excel, AWS, Spark).
* Trained and optimized **Linear**, **Lasso**, and **Random Forest** regressors using `GridSearchCV`.
* **Random Forest** performed best (MAE: 11.22).
* Developed a **Flask API** to serve predictions.

---

## 🛠️ Tech Stack

* **Language:** Python 3.7
* **Libraries:** `pandas`, `numpy`, `sklearn`, `matplotlib`, `seaborn`, `selenium`, `flask`, `pickle`, `json`
* **Install Requirements:**

  ```
  pip install -r requirements.txt
  ```

---

## 📄 References

* **Web Scraper Repo:** [GitHub](https://github.com/arapfaik/scraping-glassdoor-selenium)
* **Scraping Tutorial:** [Medium](https://towardsdatascience.com/selenium-tutorial-scraping-glassdoor-com-in-10-minutes-3d0915c6d905)
* **Flask Deployment Guide:** [Medium](https://towardsdatascience.com/productionize-a-machine-learning-model-with-flask-and-heroku-8201260503d2)
* **YouTube Walkthrough:** [Watch here](https://www.youtube.com/playlist?list=PL2zq7klxX5ASFejJj80ob9ZAnBHdz5O1t)

---

## 🧹 Data Pipeline

### 📥 Web Scraping

Collected fields:

* Title, Salary Estimate, Job Description, Rating, Company Info (Size, Revenue, HQ, etc.)

### 🧽 Data Cleaning

* Parsed salaries and ratings.
* Engineered features: Skill mentions (Python, R, Excel, AWS, Spark), location, job seniority, age of company.
* Removed rows with missing salary info.

---

## 📊 Exploratory Data Analysis

Visualized trends in salaries and job availability:

| Salary by Title                                                                                 | Jobs by State                                                                                  | Correlation Matrix                                                                                   |
| ----------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| ![Salary](https://github.com/PlayingNumbers/ds_salary_proj/blob/master/salary_by_job_title.PNG) | ![States](https://github.com/PlayingNumbers/ds_salary_proj/blob/master/positions_by_state.png) | ![Correlations](https://github.com/PlayingNumbers/ds_salary_proj/blob/master/correlation_visual.png) |

---

## 🤖 Model Building

* Converted categorical features to dummy variables.
* Trained on 80/20 train-test split.
* Models Evaluated:

  * **Linear Regression** — MAE: 18.86
  * **Lasso Regression** — MAE: 19.67
  * **Random Forest** — **MAE: 11.22** ✅

---

## 🌐 Deployment

Created a simple **Flask API** that takes job listing inputs and returns a salary estimate.
Hosted locally following [this tutorial](https://towardsdatascience.com/productionize-a-machine-learning-model-with-flask-and-heroku-8201260503d2).

---

Let me know if you'd like a badge section, screenshots, or a link to a deployed version!
"# SalarySense-Data-Science" 
