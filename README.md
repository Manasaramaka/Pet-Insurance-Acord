# 🐾 PAWSURE — Pet Insurance Data Standards Framework
> **ACORD Student Challenge 2025** | University of Connecticut | Manasa Ramaka

[![Challenge](https://img.shields.io/badge/ACORD-Student%20Challenge%202025-blue?style=flat-square)](https://www.acord.org)
[![Fields](https://img.shields.io/badge/Data%20Fields-259%20Curated-success?style=flat-square)](#dataset)
[![Categories](https://img.shields.io/badge/Categories-10-orange?style=flat-square)](#categories)
[![Outputs](https://img.shields.io/badge/Output%20Files-37-purple?style=flat-square)](#deliverables)
[![License](https://img.shields.io/badge/License-MIT-lightgrey?style=flat-square)](LICENSE)

---

## 📌 Overview

**PAWSURE** is a production-ready pet insurance data dictionary built using a hybrid AI + real-world validation methodology. The goal is to establish standardized data elements for the pet insurance underwriting industry — an $21B market growing at 12% annually — where no formal data standards currently exist.

This project was developed as a submission for the **ACORD Student Challenge 2025**, covering the full pipeline from data collection through enrichment, analytics, and API-ready output.

---

## 🎯 Project Objectives

- Identify and standardize all data fields required for pet insurance underwriting
- Validate AI-generated fields against live carrier application forms
- Curate a high-quality, production-ready dataset with rich metadata
- Deliver multiple output formats for immediate industry use

---

## 🔬 Methodology
<img width="1092" height="205" alt="image" src="https://github.com/user-attachments/assets/b057b41e-0f8c-47f4-aeeb-ab5d20f843c4" />


### Phase 1 — Data Collection
| Source | Fields Collected |
|---|---|
| GPT-5 (expert prompting) | 476 |
| Claude 3.5 (specialized prompting) | 92 |
| Carrier form validation (5 carriers) | 46 |
| **Total Raw** | **614** |

Carriers validated: **Trupanion, Healthy Paws, Fetch, Spot, ASPCA**

### Phase 2 — Processing & Enrichment
- **Deduplication** via fuzzy string matching (85% similarity threshold): 614 → 543 unique fields
- **Metadata enrichment**: 19 attributes per field including business purpose, validation rules, risk impact, regulatory compliance, ACORD standard mapping, and underwriting importance
- **Manual QC curation**: removed 35 internal processing flags and low-value duplicates → **259 final fields**

### Phase 3 — Analytics & Innovation
- 7 comprehensive analytics reports (category distribution, carrier coverage, AI prediction accuracy, completeness, risk factors, executive summary)
- Working Python risk scoring model with breed-specific risk, age curves, pre-existing conditions, geographic factors, and lifestyle indicators
- Production-ready **JSON Schema (RFC 7159)** and **OpenAPI 3.0** specifications

---

## 📊 Dataset

**Final output: 259 curated, production-ready fields across 10 categories**

<img width="1109" height="181" alt="image" src="https://github.com/user-attachments/assets/4974430f-12ac-4d2f-ba2d-c124c2574153" />

### Categories
1. Pet Information
2. Owner / Policyholder Information
3. Breed & Genetics
4. Medical History
5. Veterinary Information
6. Coverage & Policy Details
7. Claims Data
8. Geographic & Lifestyle Factors
9. Regulatory & Compliance
10. Underwriting & Risk Scoring

Each field includes **19 metadata attributes**: business purpose, data type, validation rules, risk impact rating, source classification, regulatory compliance flags, ACORD standard mapping, and underwriting importance score.

---

## ⭐ Top 40 Critical Fields

A curated subset of the **40 most critical underwriting fields** is included as a highlighted Excel sheet for quick reference and prioritized implementation.

---

## 🚀 Risk Scoring Model

A working Python model that evaluates:
- Breed-specific risk factors
- Age curves
- Pre-existing conditions
- Medical history
- Geographic risk
- Lifestyle indicators

**Outputs:** Risk score, risk tier, premium multiplier, underwriting decision

---

## 📦 Deliverables

37 production-ready output files including:

<img width="1125" height="505" alt="image" src="https://github.com/user-attachments/assets/3cb4ccd2-323d-4c79-8102-2ff21fe54d3e" />

---

## 🛠️ Tech Stack

- **Python** — data processing, fuzzy matching, risk model
- **pandas / fuzzywuzzy** — deduplication pipeline
- **OpenPyXL** — Excel output generation
- **Jupyter Notebook** — analysis & visualization
- **Matplotlib / Seaborn** — analytics charts

---

## 📁 Repository Structure

<img width="1099" height="637" alt="image" src="https://github.com/user-attachments/assets/e0f5efbb-f3db-4eb1-8263-45b20a64b4c8" />

---

## 🏃 Getting Started

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/pawsure.git
cd pawsure

# Install dependencies
pip install -r requirements.txt

# Run the risk scoring model
python models/risk_scoring_model.py

# Open the analysis notebook
jupyter notebook notebooks/pipeline.ipynb
```

---

## 👩‍💻 Author

**Manasa Ramaka**  
University of Connecticut  
ACORD Student Challenge 2025

---
     
