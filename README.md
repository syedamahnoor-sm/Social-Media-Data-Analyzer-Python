# 📊 Social Media Data Analyzer (Instagram)

## Project Overview

This project analyzes raw Instagram profile data collected from OpenAI followers. The objective is to extract useful insights from unstructured text data by parsing it into a structured format and performing exploratory analysis.

The project was completed in two phases:

1. **Initial Data Analysis** – The parsing logic was developed and tested using a small sample dataset (`Initial_data.txt`).
2. **Final Data Analysis** – The same parser was then applied to the complete dataset (`Final_data.txt`) to generate insights.

---

## Problem Statement

Imagine being given the following challenge:

> Collect raw Instagram data of OpenAI followers and answer the following questions:

- Who has the maximum number of posts?
- Who has the maximum number of followers?
- Who follows the most people?
- How many different account categories (Digital Creator, Non-Profit Organization, etc.) are present?

The dataset consists of raw Instagram profile information stored as plain text, requiring preprocessing before any analysis can be performed.

---

## Project Workflow

### 1. Data Collection

The raw Instagram profile data was collected and stored as text.

The project includes:

- `Initial_data.txt` – Sample dataset used to build and test the parser.
- `Final_data.txt` – Complete dataset used for the final analysis.

---

### 2. Data Parsing

Each Instagram profile is separated into individual chunks.

The parser extracts:

- Username
- Number of posts
- Number of followers
- Number of following
- Display name
- Account category
- Bio

The parser also converts abbreviated follower counts such as:

- `1.5K` → `1500`
- `2.3M` → `2300000`

into integer values for analysis.

---

### 3. JSON Conversion

After parsing, every profile is converted into a Python dictionary and stored inside a list.

The structured data is then exported as:

```
data.json
```

This makes the dataset reusable for future analysis and visualization.

---

### 4. Data Analysis

The project answers the following questions:

- ✅ User with the maximum number of posts
- ✅ User with the maximum number of followers
- ✅ User following the highest number of accounts
- ✅ Total number of unique account categories

---

## Project Structure

```
Social-Media-Data-Analyzer-Python/
│
├── Initial_data.txt        # Sample dataset
├── Final_data.txt          # Complete dataset
├── Parsing_Data.ipynb      # Data parsing and analysis
├── data.json               # Structured JSON output
├── README.md
└── .gitignore
```

---

## Technologies Used

- Python
- Jupyter Notebook
- JSON

Python libraries used:

- `json`

---

## Sample Output

The project identifies:

- Account with the highest number of posts
- Account with the highest number of followers
- Account following the largest number of people
- Number of unique account categories

---

## Learning Outcomes

This project helped practice:

- Text preprocessing
- String manipulation
- Data parsing
- Dictionary and list operations
- JSON serialization
- Exploratory data analysis (EDA)
- Working with unstructured datasets

---

## Future Improvements

Potential enhancements include:

- Data visualization using Matplotlib or Seaborn
- Interactive dashboard using Streamlit
- Additional statistics (average followers, top categories, follower distribution)
- CSV export support
- Automated Instagram data collection using APIs (subject to platform policies)

---

## Author

**Syeda Mahnoor**

