Welcome to my GitHub pages!

# Technical Projects

## Species at Risk (SAR) Briefing Agent (August 2026): a project of Retrieval-Augmented Generation (RAG)

- This project is about the design and implementation of a briefing agent that can answer questions about Species at Risk Act (SARA) in Canada. The agent is built using a combination of natural language processing (NLP) techniques and machine learning models to provide accurate and relevant information to users.
- The project is being implemented in multiple phases. 
  - Phase 1: A chatbot is trained on a dataset of SARA-related documents and is able to answer questions about the act completely LOCALLY, meaning that the agent can use a local LLM model running Retrival Augumented Generation (RAG) with a set of offline documents. One of the reason for doing this is to demonstrate the potential of creating AI tools without relating on external cloud-based AI service providers.
    - A recorded demo of the chatbot can be watched directly below:
      <video width="100%" controls style="max-width: 640px; display: block; margin: 15px 0; border-radius: 6px; box-shadow: 0 4px 8px rgba(0,0,0,0.15);">
        <source src="videos/chatbot_phase_1_2026-08-16.mov" type="video/quicktime">
        Your browser does not support the video tag. You can download the video [here](videos/chatbot_phase_1_2026-08-16.mov).
      </video>

## Detection and Mitigation of Data Drift and Model Decay (May-June 2022): a capstone project with partner Goldspot Discoveries Corp.

- This project is about the design and implementation of a framework in a Python package, which is generalized to all datasets and models, for monitoring and detecting data drift and model decay, i.e. when the model needs retraining. 
- The findings were presented to the geologists and data scientists of the capstone partner and received positive feedback.
- Tools/Techniques - PyTorch, Scikit-Learn, Autoencoder, PCA, confidence distribution, image properties, statistical tests, etc.

#### Project duration
- 2 months

#### Developers
Christopher Alexander, Lianna Hovhannisyan, Joshua Sia and **Steven Leung**

#### UBC Supervisor
Dr. Simon Goring

#### Advisor from Partner
Mr. Shervin Manzuri Shalmani of Goldspot Discoveries Corp.

## [Project - Cloud Deployment of Machine Learning Model](https://stevenleung2018.github.io/docs/525_project.html)

- This project is about using a publicly available large dataset, training an ensemble machine learning and deploying an API to make the model available on Amazon Web Services (AWS) for doing prediction of daily rainfall of Sydney, Australia.

#### Project duration
- 4 weeks with 4 milestones

#### AWS Services used
- EC2
- S3
- EMR (with Apache Spark)

## [DoggoDash](https://doggodash.onrender.com)

- DoggoDash is an interactive web dashboard which provides visualizations for users to explore the breeds of dogs that best match their preferences.

![DoggoDash sample screenshot](img/sketch2.png) - [GitHub repo](https://github.com/stevenleung2018/doggodash)

- Please be patient when the page loads since I am using the free tier with Render.com. 

## SQL 

I have learned SQL from UBC and have been honing my skills with exercises on platforms like LeetCode, Hackerrank, etc.  Here are some examples what the problems I solved.  I am challenging myself by trying to solve the same problem with more than one techniques (e.g. CTEs, subqueries and window functions).

Here are some examples:

- [LeetCode 1174 - Immediate Food Delivery II](https://stevenleung2018.github.io/docs/SQL/sql_leetcode_1174_Immediate_Food_Delivery_II.html)
- [LeetCode 1811 - Find Interview Candidates](https://stevenleung2018.github.io/docs/SQL/sql_leetcode_1811_Find_Interview_Candidates.html)
- [LeetCode 1097 - Game Play Analysis V](https://stevenleung2018.github.io/docs/SQL/sql_leetcode_1097_Game_Play.html)

## EDAhelper

-   Python and R packages to make Exploratory Data Analysis (EDA) easier by simplifying 4 common EDA tasks into one-line codes.
-   Presentation deck in PDF format is [here](https://stevenleung2018.github.io/docs/542_group5_EDAhelper.pdf)
-   Documentation of the Python package can be seen [here](https://pypi.org/project/edahelper/) and [here](https://edahelper.readthedocs.io/en/latest/).
-   The GitHub repo for the Python package is [here](https://github.com/UBC-MDS/EDAhelper).
-   Documentation of the R package can be see [here](https://ubc-mds.github.io/EDAhelperR/index.html).
-   The GitHub repo for the R package is [here](https://github.com/UBC-MDS/EDAhelperR).

## Is age associated with success at the Olympics?

- This is a hypothesis test of whether athletes under age 25 have a significantly higher chance of winning an Olympic medal than those age 25 or above.  It is done in the form of a reproducible data science project.
- [Non-technical report](https://stevenleung2018.github.io/docs/DSCI_542_Lab2_Report.pdf)
- [Technical report](https://stevenleung2018.github.io/docs/05_final_report.pdf)
- [GitHub repo](https://github.com/UBC-MDS/olympic_medal_htest)

