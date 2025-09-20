# Project Summary: CORD-19 Metadata Analysis

This project explores the **CORD-19 dataset** (metadata.csv), a large-scale collection of COVID-19 related research papers.

---

## Objective
- Build a **robust pipeline** for loading and analyzing large, error-prone CSV files.
- Extract **key insights** about publication activity, authorship, and content.
- Provide **visual summaries** for research trends in the COVID-19 era.

---

## Methodology
1. **Data Loading:** Multi-method approach to handle parsing errors, missing values, and large file sizes.
2. **Exploratory Data Analysis (EDA):**
   - Publication timelines
   - Journal and source breakdown
   - Text analysis of titles and abstracts
   - Collaboration trends (authors per paper)
3. **Visualization:** Rich set of plots and word clouds for interpretability.

---

## Key Findings
- **123,544 papers** analyzed from 1990–2024.
- **Pandemic years (2020–2021)** saw explosive growth in publications.
- **14,348 journals** contributed, with *Reactions Weekly* and *PLOS One* leading.
- **Collaboration:** Median 4 authors per paper, with extreme cases >3000.
- **Themes:** Titles dominated by `covid`, `patients`, `health`, `pandemic`, `study`.

---

## Impact
This analysis helps:
- **Researchers** quickly understand trends in COVID-19 literature.
- **Policy-makers** assess publication surges.
- **Data scientists** prepare for downstream NLP/text-mining of abstracts/full texts.

## Requirements
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
seaborn>=0.11.0
wordcloud>=1.9.0
