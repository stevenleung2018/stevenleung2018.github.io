---
---
---

# Project Report - Cloud Deployment of Machine Learning Model

-   Author: Steven Leung
-   Credits: project team members including Macy Chan, Zack Tang, Joyce Wang, and course instructor Dr. Gittu George

## Abstract

During the course DSCI 525 of UBC MDS 2021-22 cohort, we were tasked to deploying an Application Programming Interface (API) of an ensemble machine learning model on Amazon Web Services (AWS). The dataset was publicly available and of a fairly large size which would require the big data handling capabilities of AWS services, including EC2, S3 and EMR. The model deployed was to predict the daily rainfall in Sydney, NSW, Australia. The deployment was successful and we learned the challenges of doing so and how to take advantage of the scalability of a cloud platform like AWS for handling a large dataset.

## Background

### Team members

-   Macy Chan, Zack Tang, Joyce Wang, Steven Leung

### Project duration

4 weeks with 4 milestones

### AWS services used

-   EC2
-   S3
-   EMR (with Apache Spark)

### Languages, key packages/libraries and tools used

#### Python

-   Pandas
-   NumPy
-   urllib
-   json
-   requests
-   s3fs
-   joblib
-   scikit-learn
-   matplotlib
-   pyspark
-   flask

#### R

-   arrow
-   dplyr

#### Others

-   JupyterHub

## Project Milestones

### Milestone 1

-   Downloaded the large dataset from public location.
-   Combined the raw CSV files (with over 6 million rows of data and of total size over 6GB).
-   Performed Exploratory Data Analysis (EDA).
-   Transformed data in chunks.
-   Converted the data to various formats (including `feather`) for better performance.

### Milestone 2

-   Created an EC2 instance. ![ec2_group1](https://raw.githubusercontent.com/UBC-MDS/web_and_cloud_group_1/main/notebooks/screencap/EC2-group1.png)
-   Installed JupyterHub for collaborative development on the EC2 instance. ![jupyter_group1](https://raw.githubusercontent.com/UBC-MDS/web_and_cloud_group_1/main/notebooks/screencap/jupyter-group1.png)
-   Set up the server with shared folder. ![shared_folder](https://raw.githubusercontent.com/UBC-MDS/web_and_cloud_group_1/main/notebooks/screencap/shared_folder-group1.png)
-   Set up S3 bucket and moved data there (in `parquet` file format).
-   Got the data from S3 bucket and did data wrangling on local machine. We filtered the data so that we only modelled on the data for Sydney while the dataset had that for the whole State of New South Wales of Australia.
-   Put the filtered data (in CSV format) back to the S3 bucket. The following was what we had in the S3 bucket at the end of Milestone 2:![screen_m2_t5](https://raw.githubusercontent.com/UBC-MDS/web_and_cloud_group_1/main/notebooks/screencap/screen-milestone2-task5.png)
-   *At the end of Milestone 2, we could collaborate on the data on AWS, taking advantage of its performance and scalability.*

### Milestone 3

-   Created EMR cluster instance on AWS. ![m3_t1](https://raw.githubusercontent.com/UBC-MDS/web_and_cloud_group_1/main/notebooks/milestone3/images/Task1.png)
-   Set up browser, Jupyter environment and connect to the master node of the EMR cluster. ![m3_t2](https://raw.githubusercontent.com/UBC-MDS/web_and_cloud_group_1/main/notebooks/milestone3/images/Task2.png)
-   Developed ML models (including a Random Forest Model) using scikit-learn on local machine.\
-   Performed hyperparameter tuning using Apache Spark MLLib. The model was saved to the S3 bucket. ![m3_t3](https://raw.githubusercontent.com/UBC-MDS/web_and_cloud_group_1/main/notebooks/milestone3/images/Task3_model.png)

### Milestone 4

-   Developed API on local machine.
-   Deployed API on the EC2 instance.
-   Downloaded the model from S3 bucket to EC2 instance of the API. Here is a sample API call from a local machine to the API server on the EC2 instance: ![curl_request](https://raw.githubusercontent.com/UBC-MDS/web_and_cloud_group_1/main/notebooks/milestone4/images/curl_request.png)
-   *At the end of this Milestone, the tuned ML model has been made available with its API.*

## For more details

-   [GitHub repo](https://github.com/UBC-MDS/web_and_cloud_group_1)

### Jupyter notebooks for the Milestones

-   [Milestone 1](https://github.com/UBC-MDS/web_and_cloud_group_1/blob/main/notebooks/milestone1.ipynb)
-   [Milestone 2](https://github.com/UBC-MDS/web_and_cloud_group_1/blob/main/notebooks/milestone2.ipynb)
-   [Milestone 3](https://github.com/UBC-MDS/web_and_cloud_group_1/blob/main/notebooks/milestone3/Milestone3.ipynb)
-   [Milestone 4](https://github.com/UBC-MDS/web_and_cloud_group_1/blob/main/notebooks/milestone4/Milestone4.ipynb)
