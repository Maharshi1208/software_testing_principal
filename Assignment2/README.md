# Assignment 2: Requirements Breakdown

---

## **Table of Contents**
1. [Purpose](#purpose)
2. [Functional Requirements](#functional-requirements)
3. [System Requirements](#system-requirements)
4. [Assumptions](#assumptions)
5. [Validation Plan](#validation-plan)
6. [Task Breakdown](#task-breakdown)


---

## **Purpose**
The purpose of this assignment is to analyze the requirements for a system that assists an AI developer in generating **categorized** and **balanced training data** through **web scraping**. The system will address the client's need for **self-affirmation** (separating questions from answers) and **bias-free data** to improve AI model performance.

---

## **Functional Requirements**

### **1. Categorization of Training Questions and Answers**
**a**: The system must **categorize training questions separately from their corresponding answers**.
 **b**: Categories should be based on:
  - **Topic** (e.g., Machine Learning, Natural Language Processing).
  - **Difficulty Level** (e.g., Beginner, Intermediate, Advanced).
  - **Source of Data** (e.g., Website A, Website B).
**c**: Developers should be able to **customize categories** based on their specific needs.

### **2. Balanced Training Data**
 **a**: The system must ensure that the training data is **balanced** and free from biases.
 **b**: A **bias detection module** should analyze the dataset for imbalances in:
  - **Topic representation** (e.g., overrepresentation of one topic).
  - **Demographic biases** (e.g., gender, race).
  - **Source diversity** (e.g., data from multiple sources).
**c**: The system should provide a **balance score** for each dataset, indicating the level of bias detected.

### **3. Data Scraping and Preprocessing**
**a**: The system must **scrape data from publicly available sources** (e.g., websites, forums, or APIs).
**b**: The scraped data should be **preprocessed** to remove:
  - Irrelevant information (e.g., HTML tags, ads).
  - Duplicate content.
  - Incomplete or corrupted data.

### **4. User Feedback Mechanism**
 **a**: The system should allow developers to **provide feedback** on the quality of the categorized data.
**b**: Feedback should be used to **improve the categorization and balancing algorithms** over time.

---

## **System Requirements**

### **1. Web Scraping Module**
**a**: The system must use a **Python-based web scraping library** (e.g., BeautifulSoup, Scrapy) to extract data from publicly available sources.
 **b**: The scraping process should comply with **legal and ethical guidelines**, such as:
  - Respecting `robots.md` files.
  - Avoiding excessive requests to servers.

### **2. Categorization Module**
 **a**: The system must use **machine learning algorithms** (e.g., clustering or classification) to categorize questions and answers.
 **b**: The module should support **customizable categories** based on developer input.

### **3. Bias Detection Module**
 **a**: The system must include a **bias detection algorithm** to analyze the dataset for imbalances.
**b**: The algorithm should generate a **balance report** with:
  - Metrics for bias detection.
  - Recommendations for improving data quality.

### **4. Data Storage and Retrieval**
 **a**: The system must store categorized and balanced data in a **structured database** (e.g., MySQL, MongoDB).
**b**: Developers should be able to retrieve data using a **query interface** (e.g., SQL queries or API endpoints).

### **5. User Interface**
 **a**: The system should provide a **simple web-based interface** for developers to interact with the system.
**b**: The interface should display:
  - Categorized data.
  - Balance scores.
  - Options for providing feedback.

---

## **Assumptions**

### **1. Data Availability**
 **a**: The client has access to **publicly available data sources** for scraping.
**b**: The data sources are **reliable** and provide **sufficient training data**.

### **2. Balanced Data Definition**
 **a**: The client has a **clear definition** of what constitutes "balanced data."
**b**: The definition includes metrics such as:
  - **Equal representation of topics**.
  - **Absence of demographic bias**.
  - **Diversity in data sources**.

### **3. Infrastructure**
 **a**: The client has the necessary **infrastructure** (e.g., servers, storage) to support the scraping and categorization process.
**b**: The client’s infrastructure is **compatible** with Python-based tools and libraries.

### **4. Legal Compliance**
 **a**: The client has obtained **necessary permissions** to scrape data from publicly available sources.
 **b**: The scraping process complies with **data privacy laws** (e.g., GDPR, CCPA).

### **5. Developer Expertise**
 **a**: The client’s developers have the **necessary skills** to use the system (e.g., Python programming, database querying).
**b**: The client will provide **training** if required.

---

## **Validation Plan**

### **1. Validation of Requirements**
**a**: Review requirements with the client to ensure alignment with their expectations and goals.
**b**: Develop a **prototype** of the system (e.g., a basic web scraper and categorization module) and demonstrate it to the client.
**c**: Conduct **user acceptance testing (UAT)** with the client’s developers to ensure the system meets their needs.

### **2. Validation of Assumptions**
**a**: Validate data sources and scraping process by testing on a small dataset.
**b**: Define and test balanced data metrics with the client.
**c**: Validate infrastructure compatibility by conducting a pilot test.
**d**: Ensure legal compliance by consulting with legal experts.
**e**: Assess developer expertise and provide training if required.

---

## **Task Breakdown**

### **1. Research and Select Web Scraping Tools**
**a**: Research Python libraries for web scraping (e.g., BeautifulSoup, Scrapy).
**b**: Select the most suitable tool based on client requirements.

### **2. Develop Categorization Module**
 **a**: Implement a machine learning algorithm to categorize questions and answers.
 **b**: Allow developers to customize categories.

### **3. Implement Bias Detection Module**
 **a**: Develop an algorithm to detect biases in the dataset.
 **b**: Generate a balance report with recommendations.

### **4. Design Data Storage and Retrieval System**
 **a**: Set up a structured database (e.g., MySQL, MongoDB).
 **b**: Implement a query interface for data retrieval.

### **5. Develop User Interface**
 **a**: Create a simple web-based interface for developers.
 **b**: Integrate the interface with the categorization and bias detection modules.

### **6. Test the System**
**a**: Test the system with sample datasets.
**b**: Collect feedback from developers and make improvements.

