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

## Key Findings and Analysis

### 1. Viewing Intensity Analysis
#### Temporal Patterns
- Statistical analysis revealed intriguing patterns in viewing behavior:
  * Exam periods: 43.68 ± 46.71 videos/day (Total: 4,979 videos over 114 days)
  * Non-exam periods: 38.08 ± 33.92 videos/day (Total: 6,435 videos over 169 days)
- Despite a higher average during exam periods, Mann-Whitney U Test (p-value = 0.868) indicated no statistically significant difference in viewing intensity

#### Time Distribution
- Higher variability in viewing patterns during exam periods (SD: 46.71 vs 33.92)
- Total viewing distribution:
  * Exam periods accounted for 43.6% of total videos watched
  * Non-exam periods accounted for 56.4% of total videos watched

### 2. Content Type Analysis
#### Distribution
- Clear imbalance in content types:
  * Entertainment: 10,658 videos (93.4%)
  * Educational: 756 videos (6.6%)

### 3. Sentiment Analysis
#### Overall Distribution
- Three distinct sentiment categories emerged:
  * Neutral: 8,140 videos (71.4%)
  * Positive: 2,164 videos (19%)
  * Negative: 1,110 videos (9.6%)

#### Period Comparison
- Sentiment hypothesis testing showed no significant difference between periods
  * t-test statistic: 0.434
  * p-value: 0.665
- Both periods maintained similar emotional content distribution

### 4. Machine Learning Model Performance
#### Classification Results
- Overall accuracy: 93%
- Detailed metrics:
  * Entertainment content:
    - Precision: 94%
    - Recall: 99%
    - F1-score: 97%
  * Educational content:
    - Precision: 21%
    - Recall: 4%
    - F1-score: 6%

#### Confusion Matrix Analysis
- True Negatives (Entertainment correctly classified): 2,129
- False Positives (Incorrectly classified as Educational): 19
- False Negatives (Incorrectly classified as Entertainment): 130
- True Positives (Educational correctly classified): 5

## Main Conclusions

### 1. Viewing Pattern Analysis
My initial hypothesis suggested that viewing habits would significantly differ during exam periods. However, the data analysis revealed that despite a slightly higher average during exam periods (43.68 vs 38.08 videos per day), this difference was not statistically significant (p-value = 0.868). Interestingly, we observed greater variability in viewing patterns during exam periods (SD: 46.71 vs 33.92), suggesting that students' watching habits become less predictable during these stressful times.

### 2. Content Consumption Trends
The analysis revealed a strong preference for entertainment content across all periods, with 10,658 entertainment videos compared to 756 educational videos. This pattern persisted regardless of whether it was an exam or non-exam period. While educational content made up a smaller portion of the total viewing (6.6%), it appeared to be more focused and specifically related to academic subjects, suggesting strategic use of educational content when needed.

### 3. Model Performance and Implications
My machine learning model demonstrated exceptional accuracy in identifying entertainment content (94% precision, 99% recall), but struggled significantly with educational content classification (21% precision, 4% recall). This stark difference in performance highlights not only the class imbalance in my dataset but also suggests that educational content might be more diverse and complex to classify than initially assumed. These findings indicate a need for more sophisticated approaches to educational content detection and classification in future analyses.

## Limitations and Future Work

1. **Data Imbalance**
   - Significant disparity between entertainment and educational content
   - Need for more sophisticated classification approaches

2. **Analysis Scope**
   - Current analysis limited to basic content categorization
   - Potential for deeper analysis of video length and engagement metrics

3. **Model Improvements**
   - Consider implementing class balancing techniques
   - Explore more complex feature engineering
   - Investigate additional content categorization methods
