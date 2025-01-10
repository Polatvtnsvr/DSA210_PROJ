# Analysis of Temporal Changes in YouTube Viewing Habits in Different Periods

## Project Overview  
This project examines how my YouTube viewing habits fluctuate across different periods, with a particular focus on stressful times such as exam periods. Media consumption is often shaped by external factors like academic deadlines, holidays, or daily routines. By correlating my YouTube watch history with exam dates sourced from my Notion calendar, this study aims to uncover how viewing patterns and content preferences adapt during these times.

YouTube has become an integral part of modern life, serving as a platform for education, entertainment, relaxation, and even stress management. During exam periods, students may exhibit unique viewing behaviors—turning to entertainment for stress relief or educational content for academic support. This project seeks to answer key questions such as: 
- Does my viewing intensity increase or decrease during exam periods?  
- What types of videos do I consume more frequently—educational or entertainment content?  
- Are there shifts in the emotional tone of the videos I watch during stressful times?  

By combining my personal YouTube watch history with structured data from my Notion calendar, I aim to identify trends, patterns, and correlations in content consumption. The findings could shed light on the broader relationship between stress, time management, and media usage, offering insights into how external factors influence digital habits.  

The project will employ data science techniques such as exploratory data analysis (EDA), sentiment analysis, and thematic categorization to process and visualize the data. Results will be presented in interactive charts and dashboards, highlighting the differences in viewing habits between exam and non-exam periods. Ultimately, this project aspires to not only reveal interesting patterns in personal behavior but also contribute to a deeper understanding of media consumption during stressful periods.

---

## Motivation  
Understanding the impact of external factors, such as exams, on personal content consumption can provide deeper insights into time management, emotional states, and stress-coping mechanisms. Exam periods are often associated with increased stress and altered daily routines, which can significantly impact viewing habits.  
This project aims to uncover how my content preferences and viewing intensity change during such periods. By analyzing data from both YouTube and Notion, I aim to identify trends that help improve self-awareness, better manage stress, and balance time spent on productive and relaxing activities. The insights could also be valuable for designing personalized recommendations or behavioral models tailored to individual preferences and external conditions.

---

## Data Sources  
1. **YouTube Watch History:**  
   - Obtained via [Google Takeout](https://takeout.google.com/).  
   - Includes metadata such as video titles, watch timestamps, and durations.  

2. **Exam Dates:**  
   - Extracted from a Notion calendar using the Notion Integrations(Integrations use the API to access Notion's pages, databases, and users. like google takeout).  
   - Provides structured data on exam schedules to correlate with viewing habits.

---

## Objectives  
1. Analyze temporal viewing patterns to determine how exam and non-exam periods differ in terms of viewing intensity and timing.  
2. Examine the types of videos (e.g., education, entertainment, news) watched during exam periods compared to regular periods to identify shifts in content preferences.  
3. Perform sentiment analysis on video titles and descriptions to explore emotional patterns in content consumed during different periods.  
4. Investigate the relationship between viewing habits and stress-related periods, such as the tendency to watch short-form vs. long-form content or motivational vs. entertaining videos.  
5. Visualize all findings through charts and dashboards to effectively communicate the insights gained from the analysis.

---

## Tools and Techniques  
- **Programming:** Python (Google Colab)  
- **Libraries:** 
  - `pandas` for data processing  
  - `matplotlib` and `seaborn` for visualization  
  - `Vader` (or `TextBlob`) for sentiment analysis  
- **Data Source Integration:** 
  - Google Takeout for YouTube watch history  
  - Notion API for exam schedules  
- **Version Control:** GitHub for project documentation and code sharing  

---

## Expected Outcomes  
This analysis will provide a detailed perspective on how my YouTube viewing habits evolve during exam periods versus regular periods. I expect to uncover:  
- Variations in viewing intensity, such as increased or decreased activity during exams.  
- Shifts in content preferences, like a greater focus on entertainment for stress relief or educational videos for academic preparation.  
- Emotional patterns in video consumption, highlighting changes in the sentiment (e.g., positive, negative, neutral) of content during stressful periods.  

Visualizations will clearly communicate these findings, offering actionable insights into how external factors like exams shape digital habits. The final deliverables will include a set of interactive dashboards and a comprehensive report hosted on GitHub, providing a robust analysis of the interplay between stress, time management, and media consumption.

---

## Limitations and Future Work  
- The analysis is limited to metadata and does not include insights from the actual video content or transcripts.  
- Sentiment analysis results depend on the quality and context of video titles and descriptions, which may not always reflect the true nature of the content.  
- Future work could expand the scope by analyzing physiological data, such as stress levels, to correlate with viewing habits. Additionally, integrating transcripts or subtitles from videos could provide more robust insights into the content consumed.  
- A predictive model could be developed to forecast viewing patterns during upcoming exam periods or other stress-related times.
