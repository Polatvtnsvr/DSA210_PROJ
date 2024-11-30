# Analysis of Temporal Changes in YouTube Viewing Habits in Different Periods

## Introduction  
This project focuses on analyzing changes in my YouTube viewing habits over time, with a specific emphasis on how different periods, such as exam times, influence these habits. By correlating my YouTube watch history with external schedules, such as exam dates sourced from my Notion calendar, I aim to uncover patterns in video consumption and how content preferences shift during stressful or busy periods.

## Motivation  
Understanding the impact of external factors, such as exams, on personal content consumption can provide deeper insights into time management, emotional states, and stress-coping mechanisms. This project combines real-world data sources to analyze not only what I watch but when and why I consume specific types of content during different periods. It aims to identify trends that can help in better self-awareness and potentially optimize content consumption patterns.

## Data Sources  
1. **YouTube Watch History:**  
   - Obtained via [Google Takeout](https://takeout.google.com/).  
   - Includes metadata such as video titles, watch timestamps, and durations.  

2. **Exam Dates:**  
   - Extracted from a Notion calendar using the Notion API.  
   - Provides structured data on exam schedules to correlate with viewing habits.

## Objectives  
1. Identify temporal viewing patterns, focusing on exam and non-exam periods.  
2. Analyze sentiment of video titles and descriptions to determine emotional trends.  
3. Categorize videos into themes (e.g., education, entertainment) and compare preferences between exam and non-exam periods.  
4. Visualize changes in viewing habits and content preferences with interactive charts and dashboards.  

## Tools and Techniques  
- **Programming:** Python (Google Colab)  
- **Libraries:** `pandas`, `matplotlib`, `seaborn`, `nltk` (or `TextBlob`), `notion-client`  
- **Data Source Integration:** Google Takeout for YouTube data and Notion API for exam schedules  
- **Version Control:** GitHub for project documentation and code sharing  

## Expected Outcomes  
The analysis will reveal how my YouTube viewing habits change during different periods, such as exam times, compared to regular times. It will identify shifts in video categories, viewing times, and emotional tones, providing a comprehensive picture of the impact of external factors on my content consumption. Visualizations and a detailed report hosted on GitHub will summarize these findings, offering insights into the interplay between stress, time management, and media preferences.

## Limitations and Future Work  
- The analysis is limited to metadata and does not include video content or transcripts.  
- Future work could include comparing these findings with larger datasets or incorporating physiological data (e.g., stress levels).  
- Potential expansions could involve building a predictive model for viewing habits during upcoming stressful periods.
