# GameVerse-Analytics
This project analyzes global video game sales using Microsoft Excel. It features interactive dashboards, region-wise comparisons, genre/platform trends, and critic score evaluations. Data was cleaned and visualized using Pivot Tables, Charts, Slicers, and Conditional Formatting with custom hyperlinks for easy navigation.

## 1. Introduction
This project showcases a Microsoft Excel-created gaming sales dashboard that is both interactive and visually appealing. It is intended to examine and display data on video game sales worldwide across a range of platforms, genres, and geographical areas. In addition to showcasing the best-performing games, the dashboard makes navigation easy and intuitive by letting users interact with data using slicers, filters, and hyperlinks.

Throughout the project, a gaming-themed aesthetic has been used to boost user engagement and produce a striking visual identity. To add functionality and depth, advanced Excel features like pivot tables, dynamic charts, macros, and what-if analysis are used. These tools allow users to examine various scenarios and obtain useful insights.

This project is a fully immersive experience designed for gamers, analysts, and anyone else with an interest in numbers.

---

## 2. Source of Dataset
The dataset was sourced from:

[https://mavenanalytics.io/data-playground?order=date_added%2Cdesc&page=3&pageSize=5](https://mavenanalytics.io/data-playground?order=date_added%2Cdesc&page=3&pageSize=5)

---

## 3. Data Pre-Processing Process
A number of data preprocessing procedures were carried out to guarantee the dataset was clear, consistent, and prepared for analysis:

1. **Column Removal**:
   - The `last_update` column had over 90% missing values, making it unreliable.
   - The `img` column contained image links that were irrelevant for analysis. Both were eliminated.
   
2. **Managing Duplicate Entries**:
   - Excel's "Remove Duplicates" function was used to eliminate duplicate rows, ensuring each game entry only appeared once.

3. **Elimination of Empty Rows**:
   - Rows with blank or empty values in important columns (like `total_sales`) were removed.

4. **Resolving Missing Sales Data**:
   - Missing sales data in columns such as `na_sales`, `jp_sales`, `pal_sales`, and `other_sales` were filled with `0` to indicate no sales.

5. **Imputing Missing Critic Scores**:
   - Missing values in the `critic_score` column were replaced with the average of available scores.

6. **Formatting of Column Names**:
   - Column headers were standardized to ensure consistency and readability.

---

## 4. Analysis on Dataset

### 1. Global Sales Analysis

**Introduction**:
- The objective is to examine how video games have performed in terms of total global sales, highlighting the most successful titles in the industry.

**Tools & Functions Used**:
- **Pivot Table**: To sum `total_sales` grouped by game name.
- **Sort & Filter**: To display top-selling titles.
- **Charts**: Bar chart to visually represent the top 10 selling games.
- **Conditional Formatting**: To highlight high sales cells.

**Results**:
- Titles like `Wii Sports`, `Super Mario Bros.`, and `Mario Kart Wii` dominated the global charts.
- Nintendo and Activision emerged as strong publishers.
- Older games still hold top spots, proving their enduring popularity.

---

### 2. Regional Sales Comparison

**Introduction**:
- We analyzed how video game sales differ across regions: North America, Europe (PAL), Japan, and Others.

**Tools & Functions Used**:
- **Pivot Table**: Grouped by region (`na_sales`, `pal_sales`, `jp_sales`, `other_sales`).
- **Slicer**: To filter by platform, genre, and publisher.
- **Pie Charts & Clustered Columns** for visual comparison.

**Results**:
- North America leads in total sales.
- Japan prefers local titles, often RPGs.
- Europe shows strong performance across various genres.

---

### 3. Genre-wise Performance

**Introduction**:
- This section explores how different game genres perform in the market based on sales data.

**Tools & Functions Used**:
- **Pivot Table**: Sum of `total_sales` by genre.
- **Slicer**: Filter by year or platform.
- **Bar Chart**: For comparative view.

**Results**:
- Action and Sports are top genres globally.
- Role-playing dominates in Japan.
- Misc and Simulation genres show consistent performance.

---

### 4. Platform-wise Game Releases

**Introduction**:
- We examined the platforms on which most games were released and how well they performed in sales.

**Tools & Functions Used**:
- **Pivot Table**: Count of games by platform.
- **Bar & Line Charts**: Trend of game releases over time.
- **Slicer**: Year-wise platform filtering.

**Results**:
- Platforms like PS2 and DS have had the most game releases.
- Newer platforms show limited data but high per-title sales.

---

### 5. Hyperlink Buttons Design (User Interaction)

**Introduction**:
- We explored the design of hyperlink buttons and their placement on the page, with a focus on how they influence user navigation and interaction.

**Tools & Functions Used**:
- **Shapes (Hyperlinks)**: Buttons created as shapes with hyperlinks directing to different sections of the workbook.
- **Coloring**: Neon Blue used for shapes to ensure visibility.
- **Alignment**: Buttons aligned vertically on the left for easy access.

**Results**:
- Buttons with bright Neon Blue shapes were more visually striking, leading to higher user engagement.
- Vertical positioning near the top of the page allowed easy navigation.

---

## 5. Conclusion

The data preprocessing of the video game sales was instrumental in uncovering a plethora of information regarding the gaming business:

- The data was cleaned and pre-processed for consistency and precision, allowing for reliable analysis.
- Older games like `Wii Sports` and `Super Mario Bros.` still dominate sales charts, showing their enduring popularity.
- Regional trends revealed North America's dominance, Japan's preference for local RPGs, and Europe's diverse genre interest.
- Action and Sports games emerged as top genres globally, with Japan favoring role-playing games.
- Platforms like PS2 and DS had the most releases, but newer platforms showed strong sales per title.
- The user interface design, particularly the hyperlink buttons, significantly improved user experience by making the dashboard easy to navigate.

This project highlights how data preprocessing and targeted analysis can reveal deep insights into global video game sales trends and guide future game development strategies.

---

## 6. Future Scope

While the current analysis provides valuable insights, future improvements could include:

1. **Data Expansion**: Including data on marketing expenditure, player demographics, and online activities.
2. **Predictive Analytics**: Using machine learning to forecast future game sales.
3. **Sentiment Analysis**: Studying critic and user reviews to determine their impact on sales.
4. **Seasonal Trends**: Analyzing sales data during holiday seasons for better marketing planning.
5. **Cross-Platform Comparison**: Comparing sales for games released across various platforms.
6. **User Engagement Metrics**: Considering user reviews and social media for better sales forecasting.
7. **Enhanced Visualizations**: Using tools like Power BI or Tableau for interactive reports.
8. **External Market Forces**: Considering factors like economic conditions and alternative entertainment.
9. **Long-Term Analysis**: Conducting longitudinal studies to identify long-term trends.
10. **Expansion into Other Media**: Extending analysis to sales data from movies, TV shows, and other entertainment sectors.

---

## 7. References

1. [Maven Analytics](https://mavenanalytics.io)
2. [Kaggle](https://www.kaggle.com)
