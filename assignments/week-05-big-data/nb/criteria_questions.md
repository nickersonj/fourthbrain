# Answers to Criteria Questions

Below are my answers to questions posed in the Canvas assignment page.

## How does the Gradient-Boosted Tree Algorithm work in Classification? How does Gradient Boost differ from AdaBoost and Logistic Regression?

Gradient-boosted tree algorithms can work for classification or regression, and they use an ensemble of decision trees. It's called gradient-boosted because the algorithm tries to optimize the weak learners. AdaBoost, short for Adaptive Boosting, is adaptive because weak learners are tweaked in favor of those misclassified previously. Unlike gradient boost and AdaBoost, logistic regression is not a decision tree type algorithm and instead it is a linear model. It is specifically used for classification problems and not regression problems (despite the word "regression" in its name).

## What is a Delta Lake and how does it offer a solution to building reliable data pipelines?

Delta Lake is an optimized storage layer that is open source and compatible with Apache Spark APIs. It offers a solution to building reliable data pipelines because you can use a single copy of data for both batch operations and streaming operations. It provides incremental processing at scale.

## When working with Pandas, we use the class pandas.core.frame.DataFrame and when working with the pandas API in Spark, we use the class pyspark.pandas.frame.DataFrame, are these the same, explain why or why not?

`pandas.core.frame.DataFrame` and `pyspark.pandas.frame.DataFrame` are not the same. They are different classes; `pandas.core.frame.DataFrame` is a class from the pandas library whereas `pyspark.pandas.frame.DataFrame` is from PySpark. There are utilities to convert between these different classes of DataFrames.

## What is a Machine Learning Pipeline is and why it’s important? What are the steps in a Machine Learning workflow?

A machine learning pipeline is a series of data transformations and other steps that are performed prior to fitting the model. It's important because it allows for easy readability (so we can see exactly what operations were performed, and in what order), which means that mistakes are less likely to occur. It's also important because the same pipeline will often need to be applied to multiple sets of data, so a pipeline means you can easily apply it to a different dataset without making mistakes or copying-and-pasting. Importantly, it's less likely that data leakage will occur when you properly set up and use a pipeline.

Steps in a machine learning workflow can include: understanding the problem statement, data management, column inspection (data types, descriptive statistics, renaming), correlations, missing value imputation, feature engineering, training, hyperparameter tuning, and error analysis.
