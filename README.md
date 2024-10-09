# Machine_Learning_Tutorial

The first step if We're new to machine learning. We'll need to install Python and download a few libraries.

This Tutorial is based on the [Kaggle](https://www.kaggle.com/learn/intro-to-machine-learning) course.

## What is Machine Learning?

Machine learning is a type of artificial intelligence (AI) that provides computers with the ability to learn without being explicitly programmed. Machine learning focuses on the development of computer programs that can change when exposed to new data.

## Decision Tree

A decision tree is a flowchart-like tree structure where an internal node represents a feature(or attribute), the branch represents a decision rule, and each leaf node represents the outcome. The topmost node in a decision tree is known as the root node. It learns to partition on the basis of the attribute value.

This tutorial will have we build models as we go through following scenario:

Some friend has made millions of dollars speculating on real estate. He's offered to become business partners with us because of our interest in data science. He'll supply the money, and We'll supply models that predict how much various houses are worth.

We ask to this friend how he's predicted real estate values in the past, and he says it is just intuition. But more questioning reveals that he's identified price patterns from houses he has seen in the past, and he uses those patterns to make predictions for new houses he is considering.

Machine learning works the same way. We'll start with a model called the Decision Tree. There are fancier models that give more accurate predictions. But decision trees are easy to understand, and they are the basic building block for some of the best models in data science.

For simplicity, we'll start with the simplest possible decision tree.

It divides houses into only two categories. The predicted price for any house under consideration is the historical average price of houses in the same category.

We use data to decide how to break the houses into two groups, and then again to determine the predicted price in each group. This step of capturing patterns from data is called fitting or training the model. The data used to fit the model is called the training data.

The details of how the model is fit (e.g. how to split up the data) is complex enough that we will save it for later. After the model has been fit, We can apply it to new data to predict prices of additional homes.

## Using Pandas to Get Familiar With Your Data

The first step in any machine learning project is familiarize ourself with the data. We'll use the Pandas library for this. Pandas is the primary tool data scientists use for exploring and manipulating data. Most people abbreviate pandas in their code as pd. We do this with the command:

```python
import pandas as pd
```

The most important part of the Pandas library is the DataFrame. A DataFrame holds the type of data We might think of as a table. This is similar to a sheet in Excel, or a table in a SQL database.

Pandas has powerful methods for most things We'll want to do with this type of data.

As an example, We'll look at data about home prices in Melbourne, Australia. In the hands-on exercises, We'll apply the same processes to a new dataset, which has home prices in Iowa.

The example (Melbourne) data is loaded into a DataFrame called `melbourne_data`. We use the `head` command to see the first few rows of the data. We also use the `describe` command to see a summary of the data.

```python
melbourne_data = pd.read_csv('data/melb_data.csv')
melbourne_data.describe()
```

## Next Steps

Follow the steps in the [notebook](ml_tutorial.ipynb)