# turntable_data_analyst_assessment-
Data cleaning, aggregation, normalisation and music chart ranking analysis using SQL, Excel and PostgreSQL. 

TurnTable Data Analyst Assessment

Project Overview

This project analyzes music consumption data from multiple platforms (Radio, YouTube, and Audiomack) to create a unified chart ranking system.

The objective is to clean, aggregate, normalize, and rank songs across platforms with different consumption metrics.

---

Data Sources

Radio

Fields:

- Title
- Imps

YouTube

Fields:

- Artiste
- Song
- Difference (Streams)

Audiomack

Fields:

- play_date
- isrc
- artist
- title
- geo
- total

---

Data Cleaning Process

1. Standardized song titles using lowercase conversion.
2. Removed duplicate records through aggregation.
3. Treated missing ISRC values as null.
4. Filtered Audiomack data to Nigerian streams where applicable.
5. Merged records using standardized song titles.

---

Aggregation Methodology

Platform totals were calculated as follows:

- Radio = Sum of impressions
- YouTube = Sum of stream counts
- Audiomack = Sum of total streams

---

Normalization

Due to differences in scale across platforms, each metric was normalized using:

Normalized Score = (Value / Maximum Value) × 100


---

Output

The final output is a ranked Top 10 leaderboard based on weighted platform performance.

[youtube.csv](https://github.com/user-attachments/files/28658612/youtube.csv)
[radio.csv](https://github.com/user-attachments/files/28658611/radio.csv)
[_select_ci_Title_ci_Artiste_ci_Rank_ci_WeeksOnChart_c_Category_c_202605281627.csv](https://github.com/user-attachments/files/28658609/_select_ci_Title_ci_Artiste_ci_Rank_ci_WeeksOnChart_c_Category_c_202605281627.csv)
[Task2  by Fagbeja.docx](https://github.com/user-attachments/files/28658596/Task2.by.Fagbeja.docx)
[Task 1 by Fagbeja.docx](https://github.com/user-attachments/files/28658595/Task.1.by.Fagbeja.docx)
[merged_music_data.csv](https://github.com/user-attachments/files/28658594/merged_music_data.csv)
[turntable _project.sql](https://github.com/user-attachments/files/28658593/turntable._project.sql)
