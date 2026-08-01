# ⚽ Fantasy Premier League (FPL) 2025/26: End-to-End Data Analysis

[![Looker Studio Dashboard](https://img.shields.io/badge/Looker_Studio-View_Dashboard-blue?style=for-the-badge&logo=looker)](https://datastudio.google.com/reporting/133e2f47-8956-4153-b3f8-1538e7d258d1)

## 📌 Project Overview
This project is an end-to-end data analytics pipeline focused on the 2025/26 Fantasy Premier League (FPL) season. The goal is to move beyond basic total points and uncover underlying performance metrics, helping managers identify value picks, spot potential regressions, and make data-driven transfer decisions.

The project encompasses the full data lifecycle: from raw data extraction and cleaning via a custom Python script to data modeling and interactive visualization in Looker Studio.

## 🛠️ Tech Stack
*   **Data Extraction & ETL:** Python (Pandas), Google Colab
*   **Data Visualization & BI:** Google Looker Studio
*   **Data Processing Techniques:** Calculated Fields, `CASE` statements, Data Blending

## ⚙️ The Data Pipeline (ETL)
1.  **Extraction:** Scraped and collected raw statistical data from FPL sources using a custom Python script.
2.  **Transformation:** Cleaned and structured the dataset to isolate key metrics such as Expected Goals (xG), Hauls (high-scoring games), Blanks (1 point or fewer), and Home/Away splits.
3.  **Load & Modeling:** Connected the cleaned dataset to Looker Studio. To maintain the integrity of the original localized database while building a global-facing dashboard, I utilized dynamic Looker Studio Calculated Fields and Aliases to seamlessly translate dimensions without altering the raw data.

## 📊 Dashboard Highlights & Key Insights
The interactive Looker Studio dashboard is divided into positional analysis (Goalkeepers, Defenders, Midfielders, and Forwards) and features:

*   **xG vs. Output Analysis:** Scatter plots identifying forwards converting significantly above or below their expected metrics, signaling potential future regressions or breakout stars.
*   **The Fixture Factor:** Home vs. Away Points Per Game (PPG) comparisons, revealing which "premium" assets suffer severe drop-offs when playing on the road.
*   **Defensive Value & Attacking Returns:** Highlighting defenders who consistently deliver more attacking returns and points per Clean Sheet than their own higher-priced teammates.
*   **Haul vs. Blank Frequency:** Advanced tracking of opponent vulnerability, showcasing which teams concede the most hauls to specific positions.

## 📸 Sneak Peek
*(Adicione aqui uma captura de tela do seu dashboard usando o formato abaixo)*
`![Dashboard Screenshot](images/GK Home x Away.png)`

## 🤝 Feedback

Suggestions and feedback are always welcome.

If you have ideas for additional metrics or visualizations, feel free to open an issue or start a discussion.
