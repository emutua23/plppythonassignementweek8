# Analysis Report: CORD-19 Research Database

This report documents the results of analyzing the **CORD-19 metadata.csv** file.

---

## 1. Dataset Overview
- **Total Papers:** 123,544
- **Columns:** 19
- **Size:** ~332 MB
- **Time Range:** 1990 – 2024

---

## 2. Data Quality Assessment
- Some columns (e.g., `mag_id`, `arxiv_id`, `who_covidence_id`) were **100% missing**.
- High missingness:
  - `s2_id` (64%)
  - `pmc_json_files` (55%)
  - `pdf_json_files` (53%)
  - `sha` (53%)
- Moderate missingness:
  - `pubmed_id` (38%)
  - `pmcid` (36%)
  - `abstract` (28%)
  - `authors` (8%)
  - `journal` (3%)

---

## 3. Publication Timeline
- Extractable years for **99.6% of papers**.
- **Range:** 1990 – 2024
- **Peak Year:** 2021 (39,679 papers).
- Surge in publications around 2020–2021 reflecting COVID-19 pandemic research.

---

## 4. Journal Analysis
- **Unique Journals:** 14,348
- **Top Journal:** *Reactions Weekly* (3,191 papers).
- Other prolific journals: *PLOS One*, *BMJ*, *Nature*, *Lancet*.
- 37.6% of journals contributed only one paper → very diverse source distribution.

---

## 5. Title Analysis
- **Available Titles:** 99.9%
- **Avg. Length:** 92 chars
- **Most Frequent Words:**
  - `covid`, `patients`, `study`, `health`, `pandemic`, `case`, `review`.

- **Visualization:** Word cloud generated from 1.1M extracted words.

---

## 6. Abstract Analysis
- **Available Abstracts:** 71.9%
- **Avg. Length:** 1,451 characters.
- **Longest Abstract:** 122,392 characters.
- **Shortest Abstract:** 1 character.

---

## 7. Author Analysis
- **Available Author Info:** 91.6%
- **Avg. Authors per Paper:** 5.5
- **Median:** 4
- **Max:** 3,572
- **Single-Author Papers:** 17%

---

## 8. Data Source Analysis
- **PMC:** 64.4%
- **Medline:** 35.6%

---

## 9. File Availability
- **PDF JSON:** 47.2%
- **PMC JSON:** 44.9%
- **Both Types:** 40.3%
- **Either Available:** 51.8%

---

## 10. Visualizations Produced
- Missing data heatmaps
- Publication timeline (1990–2024, with detailed 2010+ trend)
- Top journals bar chart
- Journal diversity histogram
- Word cloud of titles
- Abstract/Title length distributions
- Author count histogram
- Data source pie + bar charts

---

## Conclusion
The analysis provides a **comprehensive view** of the CORD-19 metadata:
- Strong pandemic-driven publication spike in 2020–2021.
- Broad range of journals, but a few dominate.
- Title and abstract analyses highlight COVID-19–specific themes.
- Author patterns show collaboration-driven research.
- Over half of records contain linked full-text JSON files, enabling deeper text mining.