# Build and Deploy Text-2-SQL LLM Using OpenAI and AWS

The aim of the SQLGenPro project is to develop a Streamlit-based web application that utilizes Large Language Models (LLMs) to convert natural language queries into optimized SQL commands, enabling secure database interaction, user authentication, and seamless deployment on AWS.

## Overview
Current Industry:

In today's data-driven world, organizations across industries rely heavily on data to make informed decisions. Data is often stored in relational databases, which require SQL (Structured Query Language) to retrieve and manipulate information. However, writing SQL queries can be challenging for many professionals, especially those without a technical background, such as business analysts, product managers, or executives.

Despite the widespread availability of data, a significant bottleneck remains: the need for SQL expertise to extract meaningful insights. This creates a dependency on specialized teams, such as data analysts or engineers, to write queries and generate reports. As a result, decision-making can be delayed, and productivity hampered, particularly in situations where quick access to data is critical.

Why a Text-to-SQL Tool is Necessary:

## Data
The food delivery application database contains detailed records of users, restaurants, menu items, orders, payments, and reviews, capturing every transaction and interaction within the app. This comprehensive dataset, with tables such as Users, Restaurants, Orders, and Reviews, is designed to support the analysis of customer behaviors, service optimization, and overall business performance.

_Data is not included in this repository._

## Approach
1. Virtual Environment and Dependencies:

- Create a Python virtual environment and install necessary libraries (Streamlit, OpenAI, LangChain, database connectors).
- Configure access to Databricks and Snowflake, including connection setup and testing.
- Set up the development environment in VS Code.

2. LLM Integration and Database Interaction:

- Integrate the LLM via API to convert natural language queries into SQL.
- Develop backend modules to execute SQL queries on Databricks/Snowflake and retrieve results.
- Implement error handling to manage SQL generation and execution issues.

3. Prompt Engineering and SQL Optimization:

- Create and refine prompt templates to accurately generate SQL, including complex queries (CTEs, joins).
- Implement SQL validation and optimization to ensure generated queries are efficient and correct.

4. User Interface and Authentication:

- Build an intuitive Streamlit interface for inputting queries, displaying SQL results, and managing query history/favorites.
- Implement user authentication with secure session management and personalized experiences.

5. Advanced Query Handling and Feature Integration:

- Develop "Quick Analysis," "Deep Dive Analysis," and "Favorites" sections for enhanced user interaction.
- Test the application with complex SQL queries to ensure robustness.

6. Deployment:

- Configure and deploy the application on AWS EC2 with HTTPS for secure access and scalable performance.

Modular code overview:

Once you unzip the modular_code.zip file, you can find the following:

├─ .streamlit │   └─ config.toml ├─ Langchain_Intro.ipynb ├─ README.md ├─ SQLGenPro.png ├─ SQLGenPro.py ├─ SQLGenPro_Live.py ├─ artifacts/ ├─ authenticator.yml ├─ data/ ├─ helper.ipynb ├─ requirements.txt ├─ src │   ├─ add_logo.py │   └─ utils.py ├─ test.sql └─ utils.ipynb

Here is a brief information on the files:

## Tech stack
➔ Language: Python 3.10 ➔ Libraries: Langchain, Langchain-openai, streamlit, Databricks

➔ Model: GPT-4 ➔ Cloud Platform: Microsoft Azure and AWS

## How to run
```bash
pip install -r Code+Folder/requirements.txt
```
Notebooks: [`Langchain_Intro.ipynb`](Code+Folder/Langchain_Intro.ipynb), [`helper.ipynb`](Code+Folder/helper.ipynb), [`utils.ipynb`](Code+Folder/utils.ipynb)

## Project structure
```
.gitignore
Code+Folder/
  Langchain_Intro.ipynb
  README.md
  SQLGenPro.py
  SQLGenPro_Live.py
  authenticator.yml
  helper.ipynb
  requirements.txt
  src/
    add_logo.py
    utils.py
  test.sql
  utils.ipynb
README.md
```

## Credits
Based on a ProjectPro guided project.
