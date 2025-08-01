# Phase2_project
## MOVIE ANALYSIS PROJECT

## Business Problem  
Your company has observed that major players in the entertainment industry are creating original video content, and they want to enter this space as well. They plan to launch a new movie studio, but currently lack industry insights.

## Objective  
To explore and identify which genres or types of films perform best in terms of box office revenue and audience/critic ratings.

## Project Goal  
To determine the most successful film types based on ratings and revenue, and recommend which genres the new movie studio should focus on producing.

## Approach and Plan

### 1. Import Required Libraries  
- sqlite3 for connecting to and querying the IMDb dataset  
- pandas for data manipulation and analysis  
- matplotlib.pyplot for visualizing patterns and trends  

### 2. Load the Datasets  
- Read the IMDb .sqlite database  
- Read the Box Office Mojo .csv file  
- Display the first and last 5 rows to understand the structure  

### 3. Understand the Data  
Use exploratory methods to understand each dataset:  
- .info() to check data types and non-null counts  
- .describe() for statistical summary  
- .isna().sum() to identify missing values  

### 4. Clean the Data  
- Handle missing and inconsistent values  
- Convert columns to appropriate data types  
- Remove duplicates  
- Standardize formats. 

### 5. Merge the Datasets  
- Identify a common key to join on  
- Merge IMDb and Box Office Mojo data into a single DataFrame  

### 6. Clean the Merged Data  
- Re-check for duplicates, nulls, or type mismatches  
- Create any new relevant columns

### 7. Exploratory Data Analysis (EDA)  
Use visualizations to identify trends and patterns:  
- Top performing genres by revenue and rating  
- Correlation between budget, rating, and revenue  
- Trends over time.  
- Use bar charts, scatter plots, heatmaps, etc.  

### 8. Draw Conclusions  
Summarize key insights:  
- Which genres consistently perform well?  
- What budget levels lead to the highest returns?  

### 9. Provide Recommendations  
Suggest the best genres or film types the company should focus on producing.
__
___
## Data Cleaning  
The goal of data cleaning is to make the dataset accurate and consistent for analysis.

### 1. Handling Missing Values  
Identify and handle any null values by either dropping them or filling them using appropriate methods.

### 2. Fixing Data Types  
Convert columns to their correct data types to ensure proper analysis.

### 3. Removing Duplicates  
Drop any repeated rows to prevent skewed results.

### 4. Standardizing Text  
- Convert text to lowercase  
- Remove leading and trailing whitespace  
- Clean text columns for consistency
  
___
**Merging the two datasets**  
<br>  
The common key between the two data sets is title but they are named differently, therefore I need to rename them.  
<br>  
Merging the two data sets for analysis so as to help the head of the company identify what type of films to create.  
<br>

___
**Cleaning the merged dataframe**
___
### Visualizations

Visualizations were used to identify trends and patterns, helping to draw meaningful conclusions.

Since the goal of this analysis is to determine which types of films perform well in terms of **ratings** and **revenue**, using the IMDB and BOM datasets, the following visualizations were created:

1. **Average Revenue by Genre**  
   To identify which genres generate the highest returns.

2. **Average Rating by Genre**  
   To determine which genres are most favored by audiences.

3. **Rating vs Revenue**  
   To examine the relationship between audience ratings and box office earnings.

4. **Year vs Rating**  
   To observe how movie ratings have evolved over time.

5. **Foreign Gross vs Genre**  
   To explore how different genres perform in international markets.

___
___
### Conclusions

Based on the analysis of the IMDB and BOM datasets, it is evident that:

1. **Animation, Sci-Fi, and Adventure** genres yield the **highest returns**, while **News, War, and Romance** genres have the **least returns**.
2. **Documentaries, News, and Biographies** tend to receive the **highest ratings**, whereas **Musicals and Horror** films have the **lowest average ratings**.
3. **Highly rated movies do not always generate high revenue**, indicating that audience acclaim doesn't always

___
### Recommendations

1. **Invest in Animation and Sci-Fi genres**  
   These genres consistently deliver high returns both domestically and internationally, making them a strategic focus for future production and marketing efforts.

2. **Avoid heavy investment in News and War films**  
   These genres tend to underperform in terms of both revenue and viewer ratings, suggesting lower audience appeal and financial risk.

3. **Do not assume high ratings guarantee high revenue**  
   The analysis shows that critically acclaimed films (high ratings) do not always translate to box office success. Strategic marketing and genre appeal are also key.

4. **Prioritize Documentaries and Biographies for critical acclaim**  
   While they may not always generate the highest revenue, they tend to receive strong ratings, offering value for prestige, awards, or niche audience engagement.

5. **Expand Animation for international markets**  
   Animation performs particularly well internationally. Studios should consider scaling up animation content targeting global audiences.

6. **Leverage the steady rise in ratings since 2017**  
   The upward trend in average ratings may indicate improving film quality or shifting audience preferences. Understanding and sustaining this trend can help maintain competitive advantage.

___
**Note on the IMDB Data set**
<br>
The data set exceeds github's file size limit.Therefore I have excluded it from the repository using .gitignore.
