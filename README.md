Readme

## Required Packages
Pandas
Matplotlib
Seaborn == 0.11.0

## Project Motivation
This project is a final assignment for the Udacity Nanodegree Data Science Program. It includes a scenario were a music stream company with the name sparkify would like to find out what causes customer churn and how it can be identified in future with a train model. The data contains all user interactions with the app for a specific timeframe. Its observations therefore represent the interaction of a user within a usage session. For the training the data was aggregated and group by user id to have an summary over the total user interaction timeline. 
The steps required for the project:
-	EDA of the data to get an overview of potential relevant variables and to identify the churn event
-	Create new aggregated data set that will be used for training
-	Generate models, compare them and optimize them with a CV grid search

## Files
The main file is the jupyter notebook which included all taken steps like the EDA and the model training and additionally some images are included which are used within the notebook.

## Blog Post
To past this project additionally a blog post had to be created where the single steps and findings had to be described. This summary was published on the common platform medium and can be found [here](https://medium.com/@snagviko/prevent-your-customer-from-churning-by-in-depth-data-analysis-and-machine-learning-820e0587a3b8)

## Conclusion
To reflect the problem it is very interesting that the training happend on a aggregated data set while the EDA and the first inisghts happend on a more granular format of the underlying data. This shows that itis possible to have better insights and even a reasonable prediction accuracy in data sets that are aggregated over a wide range. Meaning that high granular observation data can and should be observed as possible to be able to make new aggregated data sets out of it that still are able to be used for predictive modelling.

It is also interesting to see how a general EDA and training approach is made with Spark. Here especially the lazy evaluation type from Spark makes some thinking required how and which functions are really necessary to use to get the required insights but also reduce the needs to generate not necessary Spark jobs that might require to much time to generate the staging and execution processes.

One difficult thing was also to make the transistion from the granular data set which had a single interaction as an observation as to a more aggregated data set which had a user as an observation. But this step was necessary, otherwise the inbalancy of the data would it even make more harder to generate a good model with a high prediction quality.
