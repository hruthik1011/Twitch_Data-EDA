# Twitch_Data-EDA

# Twitch Data Analysis

This project involves exploratory data analysis (EDA) on Twitch data, focusing on uncovering insights into viewership trends, game categories, and streamer performance. The analysis is performed using Python libraries such as Pandas, Matplotlib, and Seaborn.

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset Information](#dataset-information)
3. [Analysis Objectives](#analysis-objectives)
4. [Setup and Installation](#setup-and-installation)
5. [Key Analysis Steps](#key-analysis-steps)
6. [Results and Insights](#results-and-insights)
7. [Visualizations](#visualizations)
8. [Conclusion](#conclusion)

---

## Introduction
Twitch is a leading live-streaming platform for gamers and content creators. The dataset used in this project contains information about streams, viewers, and other metrics that help analyze popular games, peak hours, and streamer influence.

## Dataset Information
The dataset includes the following key features:
- **streamer**: The name of the Twitch streamer.
- **viewers**: Number of viewers watching the stream.
- **followers**: Total followers for the streamer.
- **category**: The game or content category being streamed.
- **stream_date**: Date of the stream.

> **Note:** Ensure the dataset is in `.csv` format for analysis.

## Analysis Objectives
1. Identify the most popular categories by viewership.
2. Analyze follower and viewer distributions.
3. Discover correlations between variables like followers and viewers.
4. Understand trends over time, such as peak streaming hours.
5. Highlight regional preferences (if location data is available).

## Setup and Installation
1. **Clone Repository**
   ```bash
   git clone <repository-url>
   cd twitch-eda
   ```

2. **Install Dependencies**
   ```bash
   pip install pandas matplotlib seaborn
   ```

3. **Run Jupyter Notebook**
   Open the provided `.ipynb` file in Google Colab or Jupyter Notebook:
   ```bash
   jupyter notebook Twitch_data.ipynb
   ```

4. **Upload Dataset**
   Ensure the dataset file (e.g., `twitch_data.csv`) is uploaded to your working directory.

## Key Analysis Steps
1. **Data Loading and Cleaning**
   - Inspect dataset structure.
   - Handle missing values and standardize column names.

2. **Univariate Analysis**
   - Analyze the distribution of viewers and followers.
   - Identify top game categories by viewership.

3. **Bivariate Analysis**
   - Explore relationships between variables like followers and viewers.
   - Compute and visualize correlations.

4. **Time-Series Analysis**
   - Examine viewership trends over time.
   - Identify peak streaming hours.

5. **Visualization**
   - Use Matplotlib and Seaborn to create insightful plots.

## Results and Insights
### Popular Categories
- Categories with the highest total viewers were identified, highlighting trends in gaming preferences.

### Viewer and Follower Trends
- Viewer count distribution reveals variations in popularity among streamers.
- Followers are strongly correlated with viewer counts, as shown in scatterplots.

### Peak Streaming Times
- Most streams occur during specific hours, aligning with user activity.

## Visualizations
Key plots generated during the analysis include:
1. **Bar Plot**: Top 10 categories by viewers.
2. **Histogram**: Distribution of followers.
3. **Scatter Plot**: Relationship between followers and viewers.
4. **Heatmap**: Correlation matrix of numeric variables.
5. **Line Plot**: Time-series trends in viewership.

### Example Code for Visualizations
```python
# Top 10 Categories by Viewers
plt.figure(figsize=(10, 6))
top_categories.plot(kind='bar', color='skyblue')
plt.title('Top 10 Categories by Viewers')
plt.xlabel('Category')
plt.ylabel('Total Viewers')
plt.show()
```

## Conclusion
This analysis provides actionable insights into Twitch's viewership patterns. Future work could include:
- Predictive modeling for viewership trends.
- Deeper regional analysis if location data is available.

---

For more details, refer to the `Twitch_data.ipynb` file.

