The Impact of Social Media Platform Usage on Daily Mood and Productivity

(Repository: platform-use-vs-mood)

🎯 Motivation

Over the past few years, I have noticed that different social media platforms affect my focus and emotions in distinct ways — for example, spending time on Instagram feels very different from watching YouTube or reading posts on X (Twitter).
This personal observation motivated me to systematically record and analyze how my daily use of these platforms relates to how I feel throughout the day.

By collecting my own data, I aim to understand whether the amount of time I spend on certain platforms has a measurable relationship with how productive, motivated, anxious, or socially comparative I feel by the end of each day.
This project combines a personal curiosity about my digital habits with data science methods to uncover meaningful behavioral patterns.

📊 Data Description

I will collect two types of data each day:

Screen time data

Daily usage (in minutes) for: Instagram, X/Twitter, YouTube, and TikTok.

Source: my phone’s Screen Time report.

Self-reported scores (1–10)

Productivity

Motivation

Anxiety

Social comparison

Each day will be recorded as one row in a CSV file.

Example data format:

date	ig_min	tw_min	yt_min	tt_min	productivity	motivation	anxiety	soc_comp	happiness
2025-11-01	75	40	60	25	7	8	3	4	8
🗓️ Data Collection Plan

Duration: 21–28 days (approximately 3–4 weeks)

Frequency: Once per day, recorded at the end of each day

Method: I will log data manually into a Google Sheet or CSV file

Backup: I will upload updated data to GitHub weekly

🧰 Tools

Python (pandas, numpy, matplotlib, scikit-learn)

Jupyter Notebook for analysis

GitHub for version control
