# Titanic ML Models 

# Introduction

Welcome to this Titanic Machine Learning Models "workbook"! Here, I will experiment with and explain a variety of machine learning models using the classic Titanic dataset from Kaggle. This notebook is designed to help one understand the following:
- how different ML algorithms work
- how to preprocess data
- how to evaluate model performance in a real-world scenario

The Titanic dataset is a well-known introductory challenge for data science and machine learning from Kaggle which gives one a great opportunity to learn about:
- Data cleaning and preprocessing
- Feature engineering
- Model selection and training
- Evaluation metrics
- Model interpretation and improvement

Throughout this workbook, I will:
- Walk through the steps of building predictive models
- Compare the performance of different algorithms
- Share insights and tips for working with tabular data

Whether you're new to machine learning or looking to deepen your understanding, this workbook will serve as a practical guide. Let's dive in and explore the world of ML with the Titanic dataset!

## Description of the Challenge

The sinking of the Titanic on April 15, 1912, is one of history's most infamous shipwrecks. Despite being considered "unsinkable," the Titanic tragically sank after hitting an iceberg, resulting in the loss of 1,502 out of 2,224 passengers and crew. While luck played a role, certain groups of people were more likely to survive than others.

The task of this project is to build a predictive model that answers the ultimate question:
 **"What sorts of people were more likely to survive?"** 
 
This data gives us access to passenger data such as their:
- name 
- age
- gender
- socio-economic class 

to make help make predictions predictions.

## Getting Started

- **Join the Competition:** Read the challenge description, accept the rules, and access the dataset.
- **Get to Work:** Download the data and build your models locally or on Kaggle Notebooks (a free, no-setup Jupyter environment with GPUs).
- **Make a Submission:** Upload your predictions to Kaggle and receive an accuracy score.
- **Check the Leaderboard:** See how your model ranks against others.
- **Improve Your Score:** Explore the discussion forums for tutorials and insights from the community.

## Resources

- [Alexis Cook’s Titanic Tutorial](https://www.kaggle.com/learn/intro-to-machine-learning): A step-by-step guide to your first submission.
- [Kaggle Lingo Video](https://www.youtube.com/watch?v=QJoa0JbuQ_o): Learn common Kaggle terminology.

## Competition Data

The Kaggle website gives us two datasets to work with for this challenge:
- **train.csv:** Contains details and survival outcomes for 891 passengers (the "ground truth").
- **test.csv:** Contains similar details for 418 passengers, but without survival outcomes. Your job is to predict these.

Use patterns found in `train.csv` to predict survival for passengers in `test.csv`. Explore the "Data" tab on Kaggle for more details.


# Titanic Dataset Data Dictionary

## Variables

- **survival**: Survival
  - 0 = No, 1 = Yes
- **pclass**: Ticket class
  - 1 = 1st, 2 = 2nd, 3 = 3rd
- **sex**: Sex
- **age**: Age in years
  - Fractional if less than 1; estimated as xx.5
- **sibsp**: Number of siblings/spouses aboard the Titanic
- **parch**: Number of parents/children aboard the Titanic
- **ticket**: Ticket number
- **fare**: Passenger fare
- **cabin**: Cabin number
- **embarked**: Port of Embarkation
  - C = Cherbourg, Q = Queenstown, S = Southampton

## Variable Notes

- **pclass**: A proxy for socio-economic status (SES)
  - 1st = Upper
  - 2nd = Middle
  - 3rd = Lower
- **age**: Age is fractional if less than 1. If the age is estimated, it is in the form of xx.5
- **sibsp**: The dataset defines family relations as:
  - Sibling = brother, sister, stepbrother, stepsister
  - Spouse = husband, wife (mistresses and fiancés were ignored)
- **parch**: The dataset defines family relations as:
  - Parent = mother, father
  - Child = daughter, son, stepdaughter, stepson
  - Some children travelled only with a nanny, therefore parch=0 for them.




## Submission Format

- Submit a CSV file with exactly 418 entries plus a header row.
- The file must have two columns:
  - `PassengerId` (any order)
  - `Survived` (1 for survived, 0 for deceased)
- Extra columns or rows will cause an error.

## Need Help?

- Visit the [Titanic Discussion Forum](https://www.kaggle.com/c/titanic/discussion) for help and insights.
- Kaggle Notebooks are a great resource for shared code and analysis.

Good luck, and enjoy your journey into machine learning with the Titanic competition!