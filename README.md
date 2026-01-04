# Netflix Movie Popularity Prediction 

## Project Overview
This is an end-to-end **Data Analysis + Machine Learning** project using Netflix movie data.  
The project starts from raw data cleaning and ends with a machine learning model that predicts **movie popularity**.

---

## Dataset
Original Netflix movie dataset containing:
- Release Date
- Title
- Overview
- Popularity
- Vote Count
- Vote Average
- Original Language
- Genre

---

## Data Cleaning
- Removed duplicate values
- Handled missing values
- Converted date column to proper format
- Cleaned multi-value genre column

---

## Exploratory Data Analysis (EDA)
Key insights from the dataset:

- **Drama** is the most frequent genre, contributing **~14%** of total movies.
- **25.5%** of movies fall under high popularity range.
- **Drama genre** contributes **~18.5%** of total popular movies.
- **Spider-Man: No Way Home** has the highest popularity score.
- **Year 2020** has the highest number of movie releases.
- Movies with higher **vote count** generally have higher popularity.

Visualizations were created using **Matplotlib and Seaborn**.

---

## Feature Engineering
- Created target column: **Popular / Not Popular**
- Applied **One-Hot Encoding** on Genre
- Selected numerical features based on correlation
- Dropped irrelevant columns

---

## Feature Scaling
- Applied **StandardScaler**
- Improved model convergence and performance

---

## Machine Learning Model
- **Problem Type:** Binary Classification
- **Model Used:** Logistic Regression
- **Why Logistic Regression?**
  - Simple and interpretable
  - Suitable for binary classification
  - Works well on structured data

---

## Model Evaluation
- Train-Test Split: 80% / 20%
- **Final Accuracy:** ~81.6%
- Evaluation Metrics:
  - Accuracy Score
  - Classification Report

---

## Prediction Use Case
**Question Answered:**  
👉 *Will a new Netflix movie be popular based on its features?*

Input Features:
- Release Year
- Vote Count
- Popularity
- Genre

Output:
- Popular (1)
- Not Popular (0)

---

## Challenges Faced & Fixes
- **Genre column mismatch during prediction**  
  → Fixed using consistent One-Hot Encoding
- **Feature mismatch errors**  
  → Solved by using pipeline and same feature set
- **Convergence warning in Logistic Regression**  
  → Fixed using feature scaling and proper preprocessing

---

## Tools & Technologies
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---


## Conclusion
This project demonstrates:
- Strong data analysis skills
- Clear understanding of EDA
- Practical machine learning implementation
- End-to-end data science workflow on real-world data

---

