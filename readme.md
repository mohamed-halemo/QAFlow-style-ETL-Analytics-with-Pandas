# 📊 QAFlow-Style ETL & Analytics + 🤖 Figma-to-QA Test Generation

This repository contains **two separate Jupyter Notebooks**, each showcasing different but complementary skills:
1. **QAFlow_ETL_Analytics.ipynb** – Data engineering & analytics with Pandas.  
2. **Figma_QA_TestGen.ipynb** – UI parsing & AI-powered QA test generation from Figma designs.

---

## 🧮 Notebook 1: QAFlow_ETL_Analytics.ipynb

This notebook demonstrates a full **ETL (Extract, Transform, Load) and analytics workflow** using **Python & Pandas**, inspired by real QAFlow-style datasets.

### 📂 Data Sources
- `test_runs.csv` – simulated test execution logs (status, duration, suite, customer ID).  
- `orders` – simulated customer subscription/order data.  
- `chat_logs.json` – simulated QA/Developer chat conversations.

### 🚀 Features
1. **ETL on Test Runs**  
   - Filter failed and flaky test runs.  
   - Add features (test name length, flaky flags).  
   - Compute suite-level metrics (fail rate, flaky rate).  
   - Save filtered/transformed data to CSV.

2. **Orders Aggregation**  
   - Aggregate total spend, average spend, max order, and order counts per customer.

3. **Chat Logs Normalization**  
   - Flatten nested JSON chat logs into a clean DataFrame.  
   - Compute session-level metrics (message count, speaker counts, conversation turns).

4. **LLM-Style Reporting**  
   - Generate a concise text summary of test suite performance, top-spending customers, and chat insights.

### 🧠 Skills Highlighted
- Advanced **pandas** (filtering, aggregation, groupby, merge, apply).  
- **JSON normalization** for nested data.  
- Feature engineering and data pipeline design.  
- Data-driven summaries ready for **LLM reporting**.

---

## 🎨 Notebook 2: Figma_QA_TestGen.ipynb

This notebook shows how to convert **Figma UI designs into AI-generated QA test cases** using Google Gemini.

### Workflow Overview
1. **Fetch Figma Design**  
   - Uses `requests` and a Figma API token to download design JSON.

2. **Explore & Parse Design**
   - Recursively walks the JSON hierarchy to list frames (screens), text layers, and UI elements.

3. **Extract Screen Elements**
   - Groups detected elements (components, instances, rectangles) and associated text under their respective screens.

4. **Prompt Gemini for Test Cases**
   - Builds a structured prompt describing screens and elements.
   - Sends it to **Gemini 2.5 Flash** to generate:
     - ✅ Step-by-step QA test scenarios.
     - 💻 Python code snippets for each test.

### Key Skills
- **API integration** with Figma (secure token handling via `.env`).  
- **Recursive JSON parsing** for UI elements.  
- **Prompt engineering** for LLMs.  
- Automated **test generation** from design assets.

---

## 🧩 How These Notebooks Complement Each Other
- **Notebook 1** focuses on **data analytics & reporting** for QA processes.  
- **Notebook 2** focuses on **design-driven QA automation** powered by AI.  
Together, they showcase **full-stack QA engineering skills**:  
from **data pipelines & insights** → to **LLM-powered test generation**.

---

## ⚡️ How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/mohamed-halemo/qaflow-etl-analytics.git
   cd qaflow-etl-analytics

## by: Mohamed Hafez