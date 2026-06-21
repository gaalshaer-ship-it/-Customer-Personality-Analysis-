# Customer Personality Analysis - Machine Learning Project

## Project Overview
This project analyzes customer data to understand customer behavior and spending patterns. Machine learning techniques were used to predict spending, classify customer responses, and segment customers into groups.

---

## 1. Data Cleaning
In this step, I cleaned the dataset by:
- Handling missing values in the Income column
- Removing or filtering unrealistic values in Age and Income
- Making sure the dataset is consistent and ready for analysis

---

## 2. Feature Engineering
I created new features to improve the analysis:
- **Age** = calculated from Year_Birth
- **TotalSpending** = total spending across all product categories
- **TotalChildren** = sum of Kidhome and Teenhome

These features helped in better understanding customer behavior.

---

## 3. Exploratory Data Analysis (EDA)
I explored the data using different visualizations:
- Histograms to understand data distribution
- Boxplots to detect outliers
- Pairplots to understand relationships between variables

From the analysis, I noticed that:
- Income has a right-skewed distribution
- Some outliers exist in Income and Age

---

## 4. Regression Models
I used regression models to predict customer TotalSpending:

Models used:
- Linear Regression
- Ridge Regression
- Decision Tree Regressor

### Results:
- Linear Regression explained most of the variance (R² ≈ 0.815)
- Ridge Regression gave similar results
- Decision Tree performed the best (R² ≈ 0.846)

So, the Decision Tree model was selected as the best regression model.

---

## 5. Classification Models
I used classification models to predict whether a customer responds to a campaign (Response).

Models used:
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Random Forest

### Evaluation metrics:
- Accuracy
- Precision
- Recall
- F1-score

### Results:
- Random Forest gave the highest accuracy
- Logistic Regression had better recall for detecting positive class
- KNN performed lower compared to other models

Due to class imbalance, recall was also an important metric to consider.

---

## 6. Clustering (Customer Segmentation)
I used K-Means clustering to group customers based on:
- Income
- Age
- TotalSpending
- TotalChildren

### Steps:
- Data scaling using StandardScaler
- Elbow method to find optimal number of clusters
- Chose k = 3
- Applied K-Means clustering

### Cluster Results:
- High-income high-spending customers
- Middle/family-oriented customers
- Low-income low-spending customers

Each cluster represents a different customer behavior group.

---

## 7. Conclusion
This project helped me understand how machine learning can be used in real-life customer analysis. It showed how we can:
- Clean and prepare data
- Build predictive models
- Classify customer behavior
- Segment customers into meaningful groups

---

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Done by
Machine Learning Student Project
