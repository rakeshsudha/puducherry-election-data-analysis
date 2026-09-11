# Puducherry Election Results 2026 — Data Analysis

## 📊 Project Overview

This project presents an Exploratory Data Analysis (EDA) of the Puducherry Election Results 2026 dataset using Python.

The objective of the project is to clean, validate, analyze, and visualize election-result data to identify meaningful patterns in candidate performance, party performance, constituency-level competition, vote distribution, and winning margins.

The analysis was performed using Python in Google Colab.

---

## 🎯 Project Objectives

The main objectives of this project are:

- Understand the structure and quality of the election dataset
- Perform data cleaning and validation
- Analyze party-wise candidate participation
- Analyze party-wise total votes
- Calculate party-wise vote share
- Analyze average votes per candidate
- Identify candidates with the highest vote totals
- Identify candidates with the highest vote percentages
- Identify winning candidates in each constituency
- Analyze party-wise constituency wins
- Calculate constituency-wise winning margins
- Identify the closest and largest-margin contests
- Compare EVM Votes and Postal Votes
- Analyze constituency-level competition
- Study the relationship between Total Votes and Vote Percentage
- Present key findings using data visualizations

---

## 🗂️ Dataset Overview

The dataset contains election-result records with the following columns:

| Column | Description |
|---|---|
| S.N. | Serial number |
| Candidate | Candidate name |
| Party | Political party / category |
| EVM Votes | Votes received through EVM |
| Postal Votes | Votes received through postal voting |
| Total Votes | Total votes received by the candidate |
| % of Votes | Candidate's vote percentage |
| Constituency | Constituency name |

### Dataset Summary

- **Total records:** 324
- **Unique candidates:** 292
- **Unique parties/categories:** 26
- **Unique constituencies:** 30

---

## 🧹 Data Cleaning & Validation

Several data-quality checks were performed before the analysis.

### Checks performed

- Data type validation
- Missing-value checks
- Duplicate-row checks
- Leading/trailing whitespace checks
- Candidate-name validation
- Party-name validation
- Constituency-name validation
- Vote percentage validation
- EVM + Postal Votes vs Total Votes validation

The vote-total validation confirmed that the EVM Votes and Postal Votes were internally consistent with the Total Votes column across the dataset.

---

## 🔍 Exploratory Data Analysis

### 1. Party Participation

Party-wise candidate participation was analyzed to understand how many candidate records were associated with each party/category.

The largest category was:

**Independent — 117 records**

Other highly represented categories included:

- None of the Above — 30
- Naam Tamilar Katchi — 28
- Tamilaga Vettri Kazhagam — 28
- Indian National Congress — 22

---

### 2. Party-wise Total Votes

Party-wise Total Votes were calculated by grouping candidates by party.

The parties with the highest total votes included:

| Party | Total Votes |
|---|---:|
| All India N.R. Congress | 200,292 |
| Indian National Congress | 151,934 |
| Tamilaga Vettri Kazhagam | 144,817 |
| Dravida Munnetra Kazhagam | 119,036 |
| Bharatiya Janata Party | 105,583 |
| Independent | 75,185 |

---

### 3. Party-wise Vote Share

Party-wise vote share was calculated based on total votes across the dataset.

The highest vote shares were:

| Party | Vote Share (%) |
|---|---:|
| All India N.R. Congress | 23.12 |
| Indian National Congress | 17.54 |
| Tamilaga Vettri Kazhagam | 16.72 |
| Dravida Munnetra Kazhagam | 13.74 |
| Bharatiya Janata Party | 12.19 |
| Independent | 8.68 |

---

### 4. Average Votes per Candidate

Average Total Votes per candidate were calculated for each party.

The highest average vote totals included:

| Party | Average Votes |
|---|---:|
| All India N.R. Congress | 12,518.25 |
| Bharatiya Janata Party | 10,558.30 |
| Latchiya Jananayaka Katchi (LJK) | 9,951.50 |
| Dravida Munnetra Kazhagam | 9,156.62 |
| Neyam Makkal Kazhagam | 7,771.50 |

This analysis provides a different perspective from total votes because it considers average candidate performance.

---

## 🏆 Candidate Performance

Candidate-level analysis was performed using Total Votes and Vote Percentage.

### Highest Total Votes

**MALLADI KRISHNA RAO**

- Party: All India N.R. Congress
- Constituency: YANAM
- Total Votes: **19,863**
- Vote Percentage: **55.44%**

### Highest Vote Percentage

**G.N.S. RAJASEKARAN**

- Party: Bharatiya Janata Party
- Constituency: THIRUNALLAR
- Total Votes: **16,829**
- Vote Percentage: **60.18%**

---

## 🗳️ Constituency-wise Winners

The winning candidate for each constituency was identified by selecting the candidate with the highest Total Votes within each constituency.

A total of **30 constituency winners** were identified.

### Party-wise Constituency Wins

| Party | Constituency Wins |
|---|---:|
| All India N.R. Congress | 12 |
| Dravida Munnetra Kazhagam | 5 |
| Bharatiya Janata Party | 4 |
| Independent | 3 |
| Tamilaga Vettri Kazhagam | 2 |
| Latchiya Jananayaka Katchi (LJK) | 1 |
| Neyam Makkal Kazhagam | 1 |
| All India Anna Dravida Munnetra Kazhagam | 1 |
| Indian National Congress | 1 |

---

## 📏 Winning Margin Analysis

Winning margin was calculated as:

**Winning Margin = Winner's Total Votes − Runner-up's Total Votes**

This analysis was used to understand the level of competition in each constituency.

### Largest Winning Margin

**KAMARAJ NAGAR**

- Winner: JOSE CHARLES MARTIN
- Winner Party: Latchiya Jananayaka Katchi (LJK)
- Winning Votes: 16,592
- Runner-up Votes: 6,387
- **Winning Margin: 10,205**

### Closest Contest

**RAJ BHAVAN**

- Winner: VIGNESH KANNAN
- Winner Party: Dravida Munnetra Kazhagam
- Winning Votes: 7,304
- Runner-up Votes: 7,017
- **Winning Margin: 287**

### Overall Winning Margin Statistics

- **Average Winning Margin:** 3,398.4
- **Smallest Winning Margin:** 287
- **Largest Winning Margin:** 10,205

---

## 🗳️ EVM Votes vs Postal Votes

The dataset contains separate EVM and Postal Vote counts.

### Overall Vote Distribution

| Vote Type | Votes |
|---|---:|
| EVM Votes | 853,899 |
| Postal Votes | 12,240 |
| Total Votes | 866,139 |

EVM Votes account for the vast majority of the recorded votes in the dataset, while Postal Votes represent a relatively small proportion.

The analysis also confirmed that:

**EVM Votes + Postal Votes = Total Votes**

---

## 🏙️ Constituency Vote Distribution

The constituencies with the highest Total Votes included:

| Constituency | Total Votes |
|---|---:|
| VILLIANUR | 39,346 |
| OZHUKARAI | 35,893 |
| YANAM | 35,826 |
| MANGALAM | 35,405 |
| ARIANKUPPAM | 34,510 |

The constituencies with the lowest Total Votes included:

| Constituency | Total Votes |
|---|---:|
| THATTANCHAVADY | 23,578 |
| MUTHIALPET | 23,560 |
| OUPALAM | 23,030 |
| ORLEAMPETH | 19,594 |
| RAJ BHAVAN | 18,716 |

---

## 📈 Correlation Analysis

The relationship between **Total Votes** and **% of Votes** was analyzed using correlation.

### Result

**Correlation: 0.982**

This indicates a very strong positive relationship between the two variables in the analyzed dataset.

The result should be interpreted in the context of how vote percentage is calculated from vote totals within constituencies.

---

## 💡 Key Findings

Some of the major findings from the analysis are:

1. The dataset contains **324 election-result records across 30 constituencies**.
2. There are **292 unique candidate names and 26 party/category values**.
3. **All India N.R. Congress** recorded the highest total votes with **200,292 votes**.
4. All India N.R. Congress also recorded the highest number of constituency wins with **12 wins**.
5. **MALLADI KRISHNA RAO** recorded the highest individual Total Votes with **19,863**.
6. **G.N.S. RAJASEKARAN** recorded the highest Vote Percentage at **60.18%**.
7. **Raj Bhavan** had the closest contest with a winning margin of **287 votes**.
8. **Kamaraj Nagar** had the largest winning margin of **10,205 votes**.
9. EVM Votes significantly exceeded Postal Votes in the dataset.
10. The correlation between Total Votes and Vote Percentage was **0.982**.

---

## 🛠️ Tools & Technologies

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Google Colab**
- **Jupyter Notebook**

---

## 📊 Analysis Workflow

```text
Data Collection
      ↓
Dataset Understanding
      ↓
Data Cleaning
      ↓
Data Validation
      ↓
Exploratory Data Analysis
      ↓
Party Analysis
      ↓
Candidate Analysis
      ↓
Constituency Analysis
      ↓
Winning Margin Analysis
      ↓
EVM vs Postal Analysis
      ↓
Correlation Analysis
      ↓
Visualizations
      ↓
Key Findings & Conclusions
