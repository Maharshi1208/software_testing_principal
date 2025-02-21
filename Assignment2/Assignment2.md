#Assignment 2: Requirements 
#Maharshi Purohit 
#8964785 
#Software engg principles

#Purpose:
We are going to further practice our requirement breakdown skills in this assignment to
include some user requirements and system based requirements.

#Scenario:
Your client is an AI developer who uses publicly available data to train their AI. They have
approached you to help them over come some of their difficulties.
The client uses a technique called web scraping to generate their training data.
You have had a few meetings with the client. At this point, you are quite confident that you
understand the challenge.
You’ve narrowed it down to the following:
- Developers want to have categorized training questions that are separate from the
answers because developers care about self-affirmation.
- Developers want to know that the training data they are using is “balanced” (does
not contain biases) because this will give them better AI models.

#Requirement Gathering
1. Understanding the Client’s Needs
The client is an AI developer who uses web scraping to generate training data. Their primary challenges are:

Categorized Training Questions: Developers want questions and answers to be separated and categorized.

Balanced Training Data: Developers want to ensure the data is free from biases to improve AI model performance.

2. Techniques for Requirement Gathering
To gather requirements effectively, use the following techniques:

Interviews: Conduct detailed interviews with the client to understand their expectations, pain points, and goals.

Questionnaires: Use structured questionnaires to collect specific information about data sources, categorization criteria, and bias detection metrics.

Observation: Observe the client’s current workflow to identify inefficiencies and areas for improvement.

Document Analysis: Review any existing documentation (e.g., data sources, scraping tools, or previous projects) to understand the current system.

3. Functional and System Requirements
Based on the client’s needs, the following requirements are gathered:

Functional Requirements
a) Categorization of Training Questions and Answers
1-The system must categorize questions and answers based on topic, difficulty level, and source of data.
2-Example: Questions related to "Machine Learning" should be grouped separately from "Natural Language Processing."

b) Balanced Training Data
1-The system must ensure that the training data is balanced and free from biases.
2-A bias detection module should analyze the data for imbalances in representation (e.g., gender, race, or topic bias).
3-The system should provide a balance score for each dataset.

c) Data Scraping and Preprocessing
1-The system must scrape data from publicly available sources (e.g., websites, forums, or APIs).
2-The scraped data should be preprocessed to remove irrelevant information (e.g., HTML tags, ads, or duplicate content).

d) User Feedback Mechanism
1-The system should allow developers to provide feedback on the quality of the categorized data.
2-Feedback should be used to improve the categorization and balancing algorithms.

4. System Requirements
a) Web Scraping Module
1-The system must use a Python-based web scraping library (e.g., BeautifulSoup, Scrapy) to extract data from publicly available sources.
2-The scraping process should comply with legal and ethical guidelines (e.g., respecting robots.md files).

b) Categorization Module
1-The system must use machine learning algorithms (e.g., clustering or classification) to categorize questions and answers.
2-The module should support customizable categories based on developer input.

c) Bias Detection Module
1-The system must include a bias detection algorithm to analyze the dataset for imbalances.
2-The algorithm should generate a balance report with recommendations for improving data quality.

d) Data Storage and Retrieval
1-The system must store categorized and balanced data in a structured database (e.g., MySQL, MongoDB).
2-Developers should be able to retrieve data using a query interface.

e) User Interface
1-The system should provide a simple web-based interface for developers to interact with the system.
2-The interface should display categorized data, balance scores, and allow feedback submission.


#Assumptions
1. Key Assumptions
a) Data Availability
1-The client has access to publicly available data sources for scraping.
2-The data sources are reliable and provide sufficient training data.

b) Balanced Data Definition
1-The client has a clear definition of what constitutes "balanced data."
2-The definition includes metrics such as equal representation of topics, absence of demographic bias, and diversity in data sources.

c) Infrastructure
1-The client has the necessary infrastructure (e.g., servers, storage) to support the scraping and categorization process.
2-The client’s infrastructure is compatible with Python-based tools and libraries.

d) Legal Compliance
1-The client has obtained necessary permissions to scrape data from publicly available sources.
2-The scraping process complies with data privacy laws (e.g., GDPR, CCPA).

e) Developer Expertise
1-The client’s developers have the necessary skills to use the system (e.g., Python programming, database querying).
2-The client will provide training if required.
