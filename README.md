# Trends in the American Beer Market: How can we help the declining beer styles to revive?


## Date story website
To learn more about this project, please visit our webpage[Let us make the most popular beer!]:beers:(https://letusmakepopularbeer.streamlit.app/).

## Abstract
This analysis aims to investigate trends in the **American beer market**, with a focus on specific regions. The study will utilize statistical and time series models to analyze these trends and make predictions.

Furthermore, sentiment analysis and natural language processing (NLP) techniques will be employed to analyze consumer comments. Through this process, the analysis will identify key trends in consumer preferences for different beer styles and show how these preferences have evolved over time. The findings will provide valuable insights for breweries and marketers in the industry, helping them to better understand the changing preferences of beer drinkers.


## Introduction
Beer is one of the world's oldest beverages, a drink that continues to evolve. While modern technology has created countless new styles and brands, many breweries still honor and preserve traditional techniques.

As a major global consumer, the United States plays a crucial role in the world's beer industry. To better understand the American beer landscape, we turned to data from BeerAdvocate, a popular website with a user base that is predominantly American. We retrieved user, brewery, and review data from the site's dataset, spanning from 1998 to 2017.

## Research questions
### 1. Identity the sentiments in users' reviews, and extract high-frequency words to obtain useful information.<br>
This analysis will investigate how consumer reviews influence beer style trends and identify the qualities that a best-selling beer should possess from a consumer perspective. Based on the findings, suggestions will be provided for beer production.

### 2. Data Visualization and Choose the popular beers<br>
This study explores the evolving popularity of top U.S. beer styles from 1998 to 2017, using the number of reviews on BeerAdvocate as a metric. The analysis will also examine the trends of the top three styles, provide future predictions, and identify their shared characteristics.

### 3. Suggestions in Brewing Beer<br>
An investigation into the relationship between beer style preference and region will be conducted. This will involve:

- Trend Analysis: Examining the evolution of beer style preferences in various regions over time.

- Data Compilation: Compiling relevant consumer preference data for regional beer trends.

- Recommendations: Generating targeted suggestions for beer production to assist breweries and sellers.


An analysis of consumer preferences for beer in different regions was conducted. All relevant data has been compiled to provide suggestions for beer production based on the findings.


## Datasets
**BeerAdvocate**

## Method
### Data preprocessing
**Data slice**
Although the initial rating data was saved in text format, they were too big to parse and analyze. Before the analysis, we used Python bash to slice and prepare the data for CSV loading by pandas.

**Clean Data**
To ensure data quality, the dataset was cleaned based on the following criteria:

- Handling Missing Values: Reviews with a missing overall score were removed. A manual check of the BeerAdvocate website confirmed that valid reviews require all five ratings: appearance, aroma, palate, taste, and overall.

- Filtering Inconsistent Data: Reviews with an inconsistent overall score were filtered out. For example, entries were considered invalid if the four component scores were all less than 3, but the overall score was greater than 4.

- Excluding Blank Reviews: Reviews that lacked any accompanying review text were also removed.


## Analytic methods<br>

- An initial statistical analysis of the pre-processed dataset was conducted to examine the relationship between the four component scores and the overall score. A statistical model was then applied to the data to gain a better understanding of consumer review trends in the U.S. beer market.<br>
<img src="Image\2.png" />


- To gain insights into consumer preferences, sentiment analysis and natural language processing (NLP) techniques were applied to the beer reviews. Specifically, the SentimentIntensityAnalyzer module from the NLTK library was used to determine the sentiment of consumer comments.The analysis also identified the most frequently mentioned keywords, providing valuable insights into consumer opinions on different beer styles.<br>

  <img src="Image\4.png" width=350 height=280/> <img src="Image\6.png" width=350 height=280/>


- Analyze the distribution of popular beers with respect to different characteristics and summarize their features. Afterwards, use data visualization techniques to select the most popular beers.<br>

  <img src="Image\7.png" />



- A further analysis will be performed on the three most popular beers in the U.S. market. A time series model will be used to forecast their future trends, with the sktime library's time series prediction module utilized to improve accuracy.<br>

  <img src="Image\8.png" /> 

- To investigate consumer preferences for beer styles in different regions, the bar_chart_race library was used to dynamically visualize how tastes have changed over time. This visualization provides a clearer understanding of evolving regional preferences, and combined with other findings, offers a basis for providing production suggestions.<br>

  ![Alt Text](https://github.com/Weijun-H/ada-2022-project-letusnameagroup/blob/main/gif/+United%20States,%20California.gif?raw=true)
  

## Proposed timeline

- 15.11.22 Slice and preprocess the dataset
- 18.11.22 Explore the factors associated with the beer ratings.
- 18.11.22 **Milestone 2** deadline
- 22.11.22 Pause project work.
- 02.12.22 **Homework 2** deadline
- 08.12.22 Begin developing a rough draft of the datastory.
- 09.12.22 Finish Statistical tests
- 11.12.22 Complete all code implementations and visualisations relevant to analysis.
- 14.12.22 Complete datastory.
- 21.12.22 Complete the website
- 23.12.22 **Milestone 3** deadline

## Organization within the team
- datastory: member 1 & 2
- website: member 3 & 4
- Code implementation: Work together
- Analysis: Group discussion
    