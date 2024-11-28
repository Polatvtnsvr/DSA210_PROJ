# Sentiment and Thematic Trend Analysis of YouTube Watch History

## Introduction  
This project explores my YouTube watch history to uncover patterns and trends in the content I consume. By analyzing the sentiment of video metadata (e.g., titles, descriptions) and categorizing themes, the project aims to gain insights into how preferences vary over time and identify key trends in my viewing habits.

## Motivation  
Understanding personal content consumption habits is crucial for better time management, self-awareness, and exploring the underlying emotional and thematic patterns in daily routines. This analysis will not only provide a deeper understanding of how I interact with content but could also pave the way for developing personalized content recommendation systems or predicting user preferences. Additionally, it is an opportunity to demonstrate practical data science skills using real-world data.

## Data Source  
The primary dataset is my YouTube watch history, obtained via [Google Takeout](https://takeout.google.com/). To enhance the dataset, video metadata such as categories, statistics (e.g., likes, views), and other relevant details will be fetched using the YouTube Data API v3.

## Objectives  
1. Conduct exploratory data analysis (EDA) to identify temporal viewing patterns (e.g., time of day, most active days).  
2. Perform sentiment analysis on video titles and descriptions to understand the emotional tone of consumed content.  
3. Categorize videos into themes (e.g., education, entertainment, news) to uncover thematic trends over time.  
4. Visualize findings using interactive charts and dashboards to present insights effectively.

## Tools and Techniques  
- **Programming:** Python (Google Colab)  
- **Libraries:** `pandas`, `matplotlib`, `seaborn`, `nltk` (or `TextBlob`) for sentiment analysis, and `wordcloud` for text visualization  
- **Data Source Integration:** Google Takeout for watch history and YouTube Data API for metadata  
- **Version Control:** GitHub for project documentation and code sharing  

## Expected Outcomes  
The project will deliver insights into my YouTube viewing habits, including the emotional tones and themes of the videos I watch. It will highlight my dominant content preferences, peak viewing times, and thematic trends over time. The final deliverables will include a set of interactive visualizations and a comprehensive report hosted on GitHub. This analysis can provide a baseline for understanding content consumption habits and pave the way for future studies or applications, such as personalized recommendations.

## Limitations and Future Work  
- The analysis is limited to video metadata and does not include the actual video content.  
- Future work could involve integrating video transcripts or employing advanced NLP techniques for deeper analysis.  
- This project could be expanded to compare viewing habits with external factors, such as holidays or significant life events.
