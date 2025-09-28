# QAFlow-style ETL & Analytics with Pandas

This repository contains a **Jupyter Notebook** that demonstrates a full **ETL (Extract, Transform, Load) and analytics workflow** using Python and Pandas, based on realistic QAFlow-style datasets. The notebook is designed to showcase skills in **data engineering, analytics, and LLM-ready reporting**, making it highly relevant for QA, AI, and data engineering roles.

---

## 📂 Contents

- `test_runs.csv` – simulated test execution logs (status, duration, suite, customer ID)  
- `orders` – simulated customer subscription/order data  
- `chat_logs.json` – simulated QA/Developer chat conversations  
- `QAFlow_ETL_Analytics.ipynb` – the main Jupyter notebook with all code, analysis, and markdown explanations

---

## 🚀 Notebook Features

1. **ETL on Test Runs**
   - Filter failed and flaky test runs  
   - Add features such as test name length and flaky flags  
   - Compute suite-level metrics (fail rate, flaky rate)  
   - Save filtered/transformed data to CSV  

2. **Orders Aggregation**
   - Aggregate total spend, average spend, max order, and order counts per customer  

3. **Chat Logs Normalization**
   - Flatten nested JSON chat logs into a clean DataFrame  
   - Compute session-level metrics (number of messages, speaker counts, average message length, conversation turns)  

4. **LLM-Style Reporting**
   - Generate a concise text summary of test suite performance, top-spending customers, and chat session insights  

---

## 🧠 Skills Demonstrated

- Advanced **pandas** usage: filtering, aggregation, groupby, merge, apply  
- **JSON normalization** for nested data  
- Feature engineering and ETL workflows  
- Summarization for **LLM-ready reports**  
- Data-driven insights for QA automation platforms  

---


## 📌 How to Run

1. Clone this repository:

```bash
git clone https://github.com/mohamed-halemo/qaflow-etl-analytics.git
cd qaflow-etl-analytics
