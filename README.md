
# platform-use-vs-mood
Comparative analysis of how different social media platforms influence daily anxiety, social comparison, productivity, and motivation.  
Self-collected dataset for DSA210 Term Project.

---

# Project Overview

This project examines how daily usage of platforms such as Instagram, X/Twitter, TikTok, and YouTube relates to different aspects of my day-to-day well-being.  
Instead of treating “social media use” as a single behavior, the project focuses on **platform-specific effects**, since each platform exposes users to different types of content, interactions, and emotional triggers.

By collecting daily screen time data together with self-reported emotional scores for 21–28 days, the goal is to understand:

- Which platforms are more strongly associated with anxiety  
- Which platforms increase social comparison tendencies  
- How different content formats relate to productivity and motivation  
- Whether long-form vs. short-form platforms affect daily mood differently  

The project uses exploratory data analysis, correlations, and simple regression models to uncover these relationships.

---

# Motivation

Over the past few years, I have noticed that different social media platforms affect my focus and emotions in distinct ways — for example, spending time on Instagram feels very different from watching YouTube or reading posts on X (Twitter).  
This personal observation motivated me to systematically record and analyze how my daily use of these platforms relates to how I feel throughout the day.

By collecting my own data, I aim to understand whether the amount of time I spend on certain platforms has a measurable relationship with how productive, motivated, anxious, or socially comparative I feel by the end of each day.  
This project brings together my personal curiosity about digital habits and data science methods to uncover potential behavioral patterns.

---

# Data Sources

The dataset used in this project is self-collected over a period of 21–28 days.  
Data comes from two main sources:

### 1. Screen Time Data
Source: **iOS Screen Time / Digital Wellbeing**

- Instagram daily usage (minutes)  
- X/Twitter daily usage (minutes)  
- TikTok daily usage (minutes)  
- YouTube daily usage (minutes)  

All values are read manually from the phone’s Screen Time dashboard.

### 2. Self-Reported Well-Being Scores
Source: **Daily self-reflection entries**

Scores recorded at the end of each day:

- Anxiety (1–10)  
- Social comparison (1–10)  
- Productivity (1–10)  
- Motivation (1–10)

### Data Storage
Data is logged manually into a CSV file or Google Sheet.  
Each row represents a single day with:

- Date  
- Platform usage metrics  
- Well-being scores  

---

# Data Description

### Screen Time Variables  
| Variable | Description |
|---------|-------------|
| ig_min | Instagram daily usage (minutes) |
| tw_min | X/Twitter daily usage (minutes) |
| tt_min | TikTok daily usage (minutes) |
| yt_min | YouTube daily usage (minutes) |

### Well-Being Variables  
| Variable | Description |
|---------|-------------|
| anxiety | Self-reported anxiety (1–10) |
| soc_comp | Self-reported social comparison (1–10) |
| productivity | Productivity of the day (1–10), supported by task completion notes |
| motivation | Motivation level (1–10) |

### Productivity definition  
Productivity is measured through a 1–10 self-report score, supported by a short “task completion note” indicating whether planned tasks for the day were completed.  
This provides additional context beyond subjective perception.

---

# Research Questions & Hypotheses

### RQ1 – Platform Use and Anxiety
**Research Question:**  
How does time spent on Instagram, X/Twitter, and TikTok relate to daily anxiety levels, and does any platform show a stronger association?

**Alternative Hypothesis (H1):**  
Higher time spent on X/Twitter will be associated with higher anxiety levels due to exposure to negative news and fast-paced content.  
Instagram and TikTok may also show positive associations, but weaker.

**Null Hypothesis (H0₁):**  
There is no relationship between daily platform usage and anxiety.

---

### RQ2 – Platform Use and Social Comparison
**Research Question:**  
How does time spent on Instagram, X/Twitter, and TikTok relate to daily social comparison tendencies?

**Alternative Hypothesis (H2):**  
Instagram and TikTok will show the strongest associations with social comparison due to curated and appearance-oriented content.  
X/Twitter is expected to show a weaker relationship.

**Null Hypothesis (H0₂):**  
There is no relationship between platform usage and social comparison.

---

### RQ3 – Platform Use, Productivity and Motivation
**Research Question:**  
How is daily time spent on YouTube, TikTok, and other platforms associated with productivity and motivation?

**Alternative Hypothesis (H3):**  
YouTube usage may be associated with higher productivity and motivation, especially when the content is educational or long-form.  
TikTok (and possibly Instagram) may predict lower productivity due to short-form, attention-demanding content.

**Null Hypothesis (H0₃):**  
Platform usage has no relationship with productivity or motivation.

---

# Expected Outcomes

Based on personal observations and general findings from digital behavior research, I expect:

- X/Twitter to show the strongest association with anxiety  
- Instagram and TikTok to show stronger links with social comparison  
- YouTube usage to correlate with higher productivity or motivation  
- TikTok usage to correlate with lower productivity due to rapid, distracting content  
- Distinct emotional patterns across platforms, supporting the idea that not all social media impacts users in the same way  

---

# Methodology

1. **Exploratory Data Analysis (EDA)**  
   - Summary statistics  
   - Distributions of usage and well-being scores  
   - Time-series plots  

2. **Correlation Analysis**  
   - Pearson/Spearman correlations  
   - Heatmaps  
   - Platform comparisons  

3. **Regression Modeling**  
   - Simple linear regression (platform → outcome)  
   - Multiple regression models including all platforms  
   - Coefficient comparisons to identify strongest predictors  

4. **Visualization**  
   - Scatter plots  
   - Line charts  
   - Bar charts comparing means across platforms  

---

# Analysis Plan

### Phase 1: Data Collection & Preprocessing  
- Daily manual logging  
- Cleaning and formatting data  
- Creating derived variables if needed  

### Phase 2: Core Analysis  
- EDA  
- Visual comparisons  
- Correlation tests  

### Phase 3: Hypothesis Testing & Modeling  
- Regression analysis  
- Comparing effect sizes  

### Phase 4: Interpretation & Reporting  
- Summary of findings  
- Limitations  
- Possible extensions  

---

# Data Collection Plan  
- **Duration:** 21–28 days  
- **Frequency:** Once per day (evening)  
- **Method:** Manual recording  
- **Backup:** Weekly GitHub updates  

---

# Tools  
- Python (pandas, numpy, matplotlib, seaborn, scikit-learn)  
- Jupyter Notebook  
- GitHub  


