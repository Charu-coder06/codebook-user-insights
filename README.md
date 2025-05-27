# 📊 CodeBook Data Analysis – Pure Python Project

**Project Type**: Individual  
**Tech Stack**: Python · JSON · Data Cleaning · Recommendation Systems  

---

## 🔍 Overview

This project simulates a **social networking platform for developers** — _CodeBook_. Using only **Python**, I performed data exploration, cleaning, and built **recommendation features** from scratch using a real-world-like JSON dataset.

Designed to demonstrate **data engineering, problem-solving, and algorithmic thinking**, this end-to-end project is structured into multiple stages reflecting practical business use cases.

---

## 🎯 Goals

- Parse and explore nested JSON data
- Clean and structure unorganized datasets
- Implement recommendation logic:
  - **People You May Know** (based on mutual friends)
  - **Pages You Might Like** (collaborative filtering)

---

## 🗂 Project Structure
📁 CodeBook-Data-Project/
- ├── codebook_data.json # Raw input data
- ├── cleaned_codebook_data.json # Cleaned output data
- ├── 1_load_display.py # Load & display users + pages
- ├── 2_clean_data.py # Data cleaning pipeline
- ├── 3_people_you_may_know.py # Mutual friend recommender
- ├── 4_pages_you_might_like.py # Page recommendation engine
- └── README.md # Project overview



---

## 🧹 Data Cleaning Summary

- Removed users with missing names
- Removed inactive users (no friends or liked pages)
- Deduplicated page records by ID
- Standardized friend lists (removed repeated IDs)

> ✅ Result: A reliable and structured dataset ready for analysis and recommendation features.

---

## 🤝 People You May Know

**Logic**: Recommends users with **mutual friends**, sorted by shared connections.

```python
find_people_you_may_know(user_id=1,data)  →  [4]
```
---

## 📄 Pages you might like

**Logic**: Uses **collaborative filtering**. If User A and B like similar pages, suggest pages B likes to A.

```python
find_pages_you_might_like(user_id=1,data)  →  [103]
```

---

## ✅ Skills Demonstrated

- Data ingestion & parsing (JSON)
- Data quality assessment & cleaning
- Graph-based recommendation logic
- User-based collaborative filtering
- Clean, modular Python code design
