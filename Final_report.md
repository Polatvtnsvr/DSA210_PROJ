# Analysis of Temporal Changes in YouTube Viewing Habits in Different Periods

## **Project Overview**
This project investigates how my YouTube viewing habits fluctuate during different time periods, with a particular focus on stressful times such as exam periods. Media consumption patterns can be influenced by external factors like academic deadlines, holidays, or daily routines. By correlating my YouTube watch history with exam dates sourced from my Notion calendar, this study aims to uncover how viewing patterns and content preferences change during these periods.

YouTube serves as a platform for education, entertainment, relaxation, and even stress management. During exam periods, students may exhibit unique viewing behaviors—turning to entertainment for stress relief or educational content for academic support. This project addresses key research questions such as:

- Does my viewing intensity increase or decrease during exam periods?
- What types of videos do I consume more frequently—educational or entertainment content?
- Are there shifts in the emotional tone of the videos I watch during stressful times?

By combining my personal YouTube watch history with structured data from my Notion calendar, I aim to identify trends, patterns, and correlations in content consumption. The findings will shed light on the broader relationship between stress, time management, and media usage, offering insights into how external factors influence digital habits.

---

## **Motivation**
Understanding the impact of external factors, such as exams, on personal content consumption provides valuable insights into time management, emotional states, and stress-coping mechanisms. Exam periods are often associated with increased stress and altered routines, which can significantly impact viewing habits. 

The primary goal of this project is to uncover how my content preferences and viewing intensity change during stressful periods. By analyzing data from both YouTube and Notion, I aim to identify patterns that promote self-awareness, help manage stress, and balance time spent on productive and relaxing activities. Additionally, these insights can contribute to personalized recommendations or behavioral models tailored to individual preferences and external conditions.

---

## **Data Sources**
### **YouTube Watch History:**
- Obtained via Google Takeout.
- Includes metadata such as video titles, watch timestamps, and durations.

### **Exam Dates:**
- Extracted from my Notion calendar using the Notion Integration (Integrations use the API to access Notion's pages, databases, and users. like google takeout).
- Provides structured data on exam schedules to correlate with viewing habits.

---

## **Objectives**
1. Analyze temporal viewing patterns to determine how exam and non-exam periods differ in terms of viewing intensity and timing.
2. Examine the types of videos (e.g., educational, entertainment) watched during exam periods compared to regular periods to identify shifts in content preferences.
3. Perform sentiment analysis on video titles to explore emotional patterns in content consumed during different periods.
4. Investigate the relationship between viewing habits and stress-related periods, such as the tendency to watch short-form vs. long-form content.
5. Visualize findings through interactive charts and dashboards to communicate insights effectively.

---

## **Tools and Techniques**
- **Programming Environment:** Python (Google Colab)

### **Data Processing & Analysis Libraries:**
  - `pandas` and `numpy` for data manipulation and numerical operations.
  - `datetime` and `timedelta` for time series processing.
  - `re` for regular expression operations.
  - `tqdm` for progress tracking.
  - `warnings` for warning management.

### **Visualization Libraries:**
  - `matplotlib` and `seaborn` for static visualizations.
  - `plotly.express` and `plotly.graph_objects` for interactive plots.

### **Text Processing & Sentiment Analysis:**
  - `BeautifulSoup` for HTML parsing.
  - `unidecode` for text normalization.
  - `vaderSentiment` for sentiment analysis.

### **Statistical Analysis:**
  - `scipy.stats` for statistical testing (`ttest_ind`, `mannwhitneyu`).

### **Machine Learning Libraries:**
  - `sklearn.model_selection` for train-test splitting.
  - `sklearn.ensemble` for Random Forest Classification.
  - `sklearn.metrics` for model evaluation metrics.

### **Data Sources & Integration:**
  - Google Takeout for YouTube watch history.
  - Notion API for exam schedules.

### **Version Control & Documentation:**
  - GitHub for code repository and version control.

---

## **Key Findings**
### **Viewing Intensity**
- The hypothesis testing showed no significant difference in viewing intensity between exam and non-exam periods.
- Daily watch patterns remained consistent, with slight variations in content types.

### **Content Preferences**
- Educational videos accounted for a larger share of watched content during exam periods.
- Entertainment videos were still watched frequently but showed minimal variation in their emotional tone.

### **Sentiment Analysis**
- During exam periods, educational videos had predominantly neutral sentiments.
- Entertainment videos had more polarized sentiments, with both positive and negative emotional tones.

---

## **Model Performance**
The Random Forest Classifier was used to predict content type based on features such as time of day, exam period, and sentiment score.
- **Accuracy:** 93%
- **Precision** (Educational Class): 21%
- **Recall** (Educational Class): 4%

### **Confusion Matrix Details:**
- **True Negative (TN):** 2129 (correctly classified as "Entertainment")
- **False Positive (FP):** 19 (incorrectly classified as "Educational")
- **False Negative (FN):** 130 (incorrectly classified as "Entertainment")
- **True Positive (TP):** 5 (correctly classified as "Educational")

---

## **Limitations and Future Work**
- **Class Imbalance:** The dataset had significantly more "Entertainment" videos than "Educational" videos, which impacted the model's ability to classify educational videos correctly. Future work should include balancing techniques such as oversampling or collecting additional educational content.
- **Sentiment Analysis:** Only video titles were used for sentiment analysis. Expanding the analysis to include subtitles, comments, or descriptions could provide more robust insights.
- **Time Period Expansion:** The analysis focused on exam periods. Including project submission dates and holiday breaks could provide additional insights into stress-related viewing patterns.
- **Model Complexity:** A simple Random Forest Classifier was used. Exploring more complex models or performing hyperparameter tuning could improve classification accuracy.

---
