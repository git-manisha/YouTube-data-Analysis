# YouTube Data Analysis Project

## Overview

This project involves analyzing YouTube video and comment data to gain insights into audience engagement, sentiment analysis, and trending video characteristics. The analysis includes text sentiment, word cloud visualization, emoji usage, and statistical relationships between various attributes of YouTube videos.

## Features

1. **Sentiment Analysis of Comments**

   - Utilize the `TextBlob` library to analyze the polarity of YouTube comments.
   - Categorize comments into positive and negative sentiment.
   - Generate word clouds for positive and negative sentiment comments.

2. **Emoji Analysis**

   - Extract emojis from comments using the `emoji` library.
   - Identify the most frequently used emojis.
   - Visualize emoji usage with bar charts.

3. **Data Cleaning**

   - Handle missing values and remove duplicates.
   - Merge multiple CSV files into a consolidated dataset.
   - Map `category_id` to meaningful category names using a JSON file.

4. **Audience Engagement Metrics**

   - Calculate engagement rates such as `likes_rate`, `dislikes_rate`, and `comment_count_rate`.
   - Explore relationships between engagement metrics and categories.

5. **Visualization**

   - Create visualizations using `matplotlib`, `seaborn`, and `plotly` to:
     - Compare engagement across video categories.
     - Analyze correlation between `views`, `likes`, and `dislikes`.
     - Identify channels with the largest number of trending videos.

6. **Punctuation Analysis**

   - Analyze the relationship between the number of punctuation marks in titles/tags and metrics such as `views`, `likes`, and `comments`.

## Libraries Used

- **Data Handling:** `pandas`, `numpy`
- **Visualization:** `matplotlib`, `seaborn`, `plotly`
- **Text Analysis:** `TextBlob`, `wordcloud`
- **Emoji Analysis:** `emoji`
- **File Handling:** `os`

## Dataset

The project uses:

- **Comments Data:** `UScomments.csv`
- **Video Data:** Multiple CSV files in the `videodata` folder.
- **Category Mapping:** `US_category_id.json`

## Steps to Run

1. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn textblob wordcloud emoji plotly
   ```
2. Clone the repository and navigate to the project folder:
   ```bash
   git clone https://github.com/your-repo/youtube-data-analysis.git
   cd youtube-data-analysis
   ```
3. Ensure the dataset files are in the correct directory structure as mentioned in the code.
4. Run the Python script to generate insights and visualizations.

## Insights

- Sentiment analysis helps identify the overall audience reaction.
- Emoji usage provides additional context about viewer sentiments.
- Categories with higher engagement rates can be targeted for content strategy.
- Punctuation in titles/tags may correlate with higher/lower views and likes.

## Visualization Examples

- Word clouds for positive and negative comments.
- Bar charts for top channels based on trending videos.
- Box plots comparing engagement metrics across categories.
- Heatmaps showing correlation between views, likes, and dislikes.

## Future Work

- Extend analysis to global YouTube datasets.
- Perform advanced NLP techniques for more accurate sentiment analysis.
- Explore time-series analysis of trending video data.

## Folder Structure

```
YouTube Data Analysis
├── UScomments.csv
├── videodata/
│   ├── video1.csv
│   ├── video2.csv
│   └── ...
├── US_category_id.json
├── youtube_data_analysis.py
└── README.md
```

## Author

Manisha Soni

