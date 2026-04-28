# Deep Learning Challenge: Charity Funding Success Prediction

## Project Overview

This project uses a **deep learning neural network** to predict whether nonprofit organizations funded by a foundation will successfully use their funding.

Using historical application data from the **Alphabet Soup Foundation**, I built and optimized a binary classification model that helps identify which organizations are most likely to achieve successful outcomes after receiving financial support.

This project demonstrates my ability to combine:

- machine learning modeling  
- data preprocessing  
- model optimization  
- business-focused interpretation  

to solve a real-world prediction problem.

---

## Business Problem

Nonprofit organizations often apply for funding, but not every funded organization delivers successful results.

The challenge was to build a model that could answer:

**Can historical applicant data predict whether a funding applicant will be successful?**

A predictive model like this could help organizations:

- improve funding decisions  
- reduce financial risk  
- prioritize stronger applicants  
- allocate resources more effectively  

---

## Business Value

This project shows how deep learning can support better decision-making by helping stakeholders:

- identify high-potential applicants  
- reduce inefficient spending  
- improve grant allocation strategy  
- automate parts of the review process  

Rather than relying only on manual review, organizations could use predictive analytics to support funding decisions at scale.

---

## Technical Skills Demonstrated

### Machine Learning
- Binary classification
- Neural network design
- Model tuning
- Performance evaluation

### Data Preparation
- Feature engineering
- One-hot encoding
- Data normalization
- Handling high-cardinality features

### Tools & Technologies
- Python
- TensorFlow / Keras
- Scikit-learn
- Pandas
- Jupyter Notebook

Examples:
:contentReference[oaicite:0]{index=0}  
:contentReference[oaicite:1]{index=1}  
:contentReference[oaicite:2]{index=2}  

---

## Dataset

The dataset includes historical records such as:

- application type  
- affiliation  
- organization classification  
- income amount  
- special considerations  
- funding amount requested  
- organization success status  

The target variable was:

**IS_SUCCESSFUL**
- 1 = successful
- 0 = unsuccessful

---

## Project Workflow

### 1. Data Cleaning
Removed non-beneficial identifier columns such as:

- EIN
- NAME

### 2. Feature Engineering
- Binned rare categorical values
- Encoded categorical variables
- Split features and target variables

### 3. Data Scaling
Standardized numerical features to improve model performance.

### 4. Model Building
Created a neural network with:
- input layer
- hidden layers
- output layer for binary prediction

### 5. Model Optimization
Improved performance by adjusting:
- number of neurons
- hidden layers
- activation functions
- training epochs

---

## Model Results

Two models were developed:

### Initial Model
- Baseline neural network
- Measured initial predictive accuracy

### Optimized Model
- Additional tuning
- Improved classification performance
- Better generalization on unseen data

Repository files include:
- `AlphabetSoupCharity.ipynb`
- `AlphabetSoupCharity_Optimization.ipynb`
- trained `.h5` model files :contentReference[oaicite:3]{index=3}

---

## Key Findings

### Predictive Insights
The model identified patterns showing that:

- certain organization types had higher success rates  
- applicant income influenced outcomes  
- classification categories impacted funding performance  

### Technical Insights
Model tuning improved performance by:

- reducing underfitting
- improving validation accuracy
- strengthening prediction reliability

---

## Why This Project Matters

This project demonstrates my ability to:

✅ prepare messy data for machine learning  
✅ build neural network models  
✅ improve model performance  
✅ explain technical work in business terms  
✅ connect analytics to organizational decision-making  

These skills are valuable in roles such as:

- Data Analyst  
- Machine Learning Analyst  
- Junior Data Scientist  
- Analytics Engineer  

---

## Repository Structure

```bash
deep-learning-challenge/
│── AlphabetSoupCharity.ipynb
│── AlphabetSoupCharity_Optimization.ipynb
│── AlphabetSoupCharity.h5
│── AlphabetSoupCharity_Optimization.h5
│── AlphabetSoup_Analysis.md
│── README.md
