# BERT-for-NLU-in-SQL

This repository shows how ML techniques can be integrated with database for query optimization. Moreover it shows how to leverage BERT model for Text to SQL generation allowing users to write sql query without having to know proper syntax.


# Techniques Used:
1. Data storage in PostGreSQL.

2. Schema Matching with BERT using cosine similarity.

3. Query Optimization using embeddings for efficient search.

4. Clustering to group similar columns.

5. Dynamic Model update tracking by checking database.

6. Text to SQL generation by extracting intent from text based query and performing cosine similarity against schema embeddings.


# Setup:
1. Download the dataset from ths link: https://www.kaggle.com/datasets/hoixding/store-sales-in-tpc-ds-v32-1gb

2. Download postgresql.

3. Create database by opening SQL shell(psql) and running the command CREATE DATABASE tpc_ds. Connect to this database using \c tpc_ds;

4. Create tables current schema and simulated schema and load the downloaded dataset in these tables.

5. Ensure python is installed and run pip install -r requirements.txt.



# Results:
1. Query Optimzation using BERT Embeddings:
   
   <img width="323" alt="image" src="https://github.com/user-attachments/assets/14b3682a-e553-4003-bc9c-260ce07cdd96" />


2. TEXT based query to SQL:



<img width="642" alt="image" src="https://github.com/user-attachments/assets/640adc46-aa5c-4ff2-ac10-9db6880e3d7f" />

