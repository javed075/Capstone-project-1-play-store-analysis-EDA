# Capstone-project-1-play-store-analysis-EDA
# Problem Statement
To explore and analyze the data to discover key factors responsible for app engagement and success. Our mission is to assist Android developers in understanding what is the motivating factor for people to download an app. Finding out what influences a person's decision to download an app will be helpful as well.

# Business Objectives Through Google Play Store Data Analysis
This repository focuses on the exploration and analysis of data from the Google Play Store to achieve various key business objectives. By delving into the wealth of information available, we aim to unlock valuable insights that can guide strategic decisions and drive success in the app market. Some potential business objectives that can be achieved through this data analysis include:

1. **Identifying App Trends and Opportunities:**
   Through a comprehensive analysis of app download and usage patterns, businesses can identify emerging trends and lucrative opportunities within the dynamic app market. By recognizing which types of apps are gaining popularity, we can assist in guiding informed decisions regarding app development and innovation.

2. **Understanding User Demographics:**
   Utilizing Play Store data, businesses gain access to user demographics encompassing factors such as age, gender, location, and interests. This invaluable insight empowers targeted marketing campaigns and enables the customization of app experiences tailored to specific user segments.

3. **Enhancing App Performance:**
   By meticulously analyzing metrics such as app crashes and user reviews, businesses can identify areas for improvement within their apps. This data-driven approach facilitates the enhancement of app performance, resulting in an optimized user experience and heightened satisfaction.

4. **Exploring Monetization Avenues:**
   The analysis of user behavior and engagement data offers businesses a window into new monetization opportunities within their apps. From in-app purchases to strategic advertising placements, these insights can foster innovative revenue streams.

By engaging in this data-driven exploration, we aim to provide businesses with a clearer understanding of their app users, while also empowering them to make informed decisions that contribute to the growth and success of their app ventures.

# Variables-
- **App**: The name of the application listed on the Google Play Store.
- **Category**: The thematic classification of the app, aiding users in navigation and discovery.
- **Rating**: The average user rating given to the app, reflecting its perceived quality.
- **Reviews**: The count of user reviews, offering insight into the app's popularity and user engagement.
- **Size**: The space occupied by the app on a device, influencing installation decisions.
- **Installs**: The approximate number of times the app has been downloaded, indicating its reach.
- **Type**: Denotes whether the app is free or paid, impacting user acquisition strategy.
- **Price**: The cost of the app if it's not free, affecting user adoption.
- **Content Rating**: Provides information about the suitability of the app's content for different audiences.
- **Genres**: Describes the app's genre or category in more detail, aiding user exploration.
- **Last Updated**: Indicates when the app was last updated, reflecting maintenance and improvements.
- **Current Ver**: Specifies the current version of the app, relevant for feature tracking.
- **Android Ver**: The minimum Android version required to run the app, guiding compatibility considerations.

By above to method we know that we have 13 column 12 have object data type and one column that is Rating has float data type.
by describe method we calculate the mean, count,standard deviation,min value,max value and percentile value.
The variation between avg and max value is very lage. it indicate that there is must present outliers.

# Data Wrangling
Data wrangling in Python involves transforming and preparing raw data into a structured, usable format for analysis. This process encompasses tasks like cleaning, handling missing values, formatting, merging datasets, and feature engineering. Libraries like Pandas provide powerful tools to manipulate data frames, perform filtering, aggregation, and create visualizations. Effective data wrangling ensures data quality, facilitating meaningful insights and informed decision-making in subsequent analyses.

Sure, here's the data wrangling process you described, broken down into bullet points:

1. **Handling Null Values in Rating Column:**
   - Replace null values in the "Rating" column with the median of that column.

2. **Handling Null Values in Other Columns:**
   - Replace null values in other columns with the previous non-null value of that column.

3. **Converting Data Types:**
   - Convert the following columns' data types to appropriate types:
     - **Size:**
       - Since the "Size" column contains values in both "M" (megabytes) and "K" (kilobytes), as well as "varies with device," convert the values to megabytes (MB) for uniformity.
       - Convert the column to float data type.
     - **Installs:**
       - Remove any "+" and "," symbols from the "Installs" column and convert it to a float data type.
     - **Price:**
       - Remove the "$" symbol from the "Price" column and convert it to a float data type.

# Exploratory Data Analysis:
Exploratory Data Analysis (EDA) in Python involves analyzing and summarizing data to understand its main characteristics, relationships, and patterns. It employs various techniques such as data visualization, statistical measures, and data manipulation to gain insights and identify potential trends or anomalies within the dataset. EDA helps researchers and analysts make informed decisions about data preprocessing, feature selection, and modeling strategies by revealing hidden insights that aid in forming hypotheses and guiding further investigation.

**Problem Statement:**
Identify key insights from an exploratory data analysis (EDA) of a Google Play Store apps dataset and provide concise answers to relevant questions.

**Answers from EDA:**
1. Q: Which categories dominate the Google Play Store?
   A: Family, Game, and Tools are the most prevalent categories, while Comics and Beauty have the lowest representation.

2. Q: What are the top categories in terms of contribution?
   A: The top 10 categories are led by Family (29%) and Game (17%).

3. Q: Which category has the highest number of installations?
   A: The Game category stands out as the most installed.

4. Q: How do app prices vary across categories?
   A: Apps in Finance and Lifestyle categories tend to have higher prices.

5. Q: What's the review distribution among Game category apps?
   A: Game category apps receive significantly higher reviews on average.

6. Q: What portion of apps are free?
   A: Around 93% of the apps are available for free.

7. Q: Which games have the highest installations?
   A: SUBWAY SURFERS, CANDY CRUSH SAGA, TEMPLE RUN 2, and POU are the top installed games.

8. Q: How are Installs and Reviews related?
   A: Installs and Reviews exhibit a strong positive correlation, as shown in the heatmap and regression plot.

9. Q: What's the distribution of content ratings?
   A: Majority of apps fall under the "Everyone" content rating, with fewer apps rated as "Adult" or "Unrated".

10. Q: How do app sizes vary?
    A: About 50% of apps range between 5 MB and 30 MB, while some exceed 70 MB in size.

11. Q: What's the distribution of positive reviews?
    A: Positive reviews account for approximately 63% of the total reviews.

**Summary:** Through EDA, it's evident that certain categories dominate the Play Store, with Family and Game being prominent. Positive reviews are prevalent, and there's a correlation between Installs and Reviews. Most apps are free, but pricing varies across categories. Content ratings mainly fall under "Everyone". A clear picture emerges about app size and top installed games. These insights drive better understanding for app developers and users alike.

# Solution to Business Objective-
Certainly, here's a concise version of the potential suggestions based on the business objectives:

1. **Optimize Category Selection:** Focus on app categories like Family and Game, which are popular and have high user engagement, increasing the likelihood of app success.

2. **Innovative Features:** Explore innovative features that set the app apart from competitors, attracting a dedicated user base within the popular categories.

3. **Enhance User Experience:** Leverage user reviews and ratings to pinpoint areas for improvement, ensuring a better user experience and higher overall satisfaction.

4. **Effective Pricing:** Analyze successful apps' pricing models and adjust your app's pricing strategy to align with market trends, enhancing its attractiveness to potential users.

# Conclusion
here are the suggestions derived from the conclusions drawn after analyzing the datasets. These suggestions aim to assist the Play Store company in making informed decisions for better outcomes:

1. **Diverse App Portfolio:**
   - **Beneficial for Developers:** Focus on introducing high-quality game apps with suitable sizes, considering the Game category's substantial user engagement. This can lead to rapid growth and increased user adoption.

2. **Quality and Popularity:**
   - **Beneficial for Customers:** Prioritize game apps due to their high popularity and engagement. Users can expect a satisfying experience within this category.

3. **Informed Decision-Making:**
   - **Beneficial for Customers:** Empower users with valuable insights regarding app categories, free and paid app proportions, and average app sizes. This data can guide their app download choices effectively.

4. **Targeted Development:**
   - **Beneficial for Developers:** Recognize the significance of the Game and Family categories in terms of installations. Focusing on these categories can lead to higher app adoption rates.

5. **Enhanced Revenue Potential:**
   - **Beneficial for Developers:** Recognize the potential in the Finance and Lifestyle categories due to their higher-priced apps. Developers could consider optimizing app offerings within these categories.

6. **Strategic Game Selection:**
   - **Beneficial for Developers:** Concentrate on developing or promoting games like SUBWAY SURFERS, CANDY CRUSH SAGA, TEMPLE RUN 2, and POU, which have demonstrated high installations and popularity.

7. **Cater to User Preferences:**
   - **Beneficial for Developers:** Capitalize on the demand for Game and Family apps by focusing on these categories during app development.

8. **Balanced Monetization Strategy:**
   - **Beneficial for Developers and Customers:** Recognize the customer preference for free apps and maintain a balanced mix of free and paid apps to cater to varying user segments.

9. **Content Rating Alignment:**
   - **Beneficial for Developers:** Acknowledge the predominance of "Everyone" content ratings and align app development efforts accordingly, ensuring broader accessibility.

By considering these suggestions, the Play Store company can make more informed decisions that enhance user experience, increase app adoption, and improve overall revenue generation.
