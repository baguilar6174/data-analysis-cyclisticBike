# [Cyclistic bike-share Analysis Case Study](https://www.kaggle.com/code/bryana/cyclistic-bike-share-analysis)

This project involves analyzing the bike trip data from Cyclistic, a bike-share company based in Chicago, to understand the behavior of its riders and identify opportunities for optimizing marketing strategies. The analysis aims to differentiate between annual members and casual riders, uncover usage patterns, and provide insights to guide business decisions. This case study is about a fictitious company, Cyclistic. Where I will answer business questions, following the steps of the data analysis process: Ask, Prepare, Process, Analyze, Share and Act.

## Scenario

Cyclistic's marketing director believes that the company's future success depends on maximizing the number of annual members. Therefore, his team wants to understand how casual users and annual members use Cyclistic's bikes differently. From this information, his team will design a new marketing strategy to convert occasional riders into annual members. But first, Cyclistic executives must approve their recommendations, so they must be backed by compelling data and professional data visualizations.

## About the company

In 2016, Cyclistic launched a successful bike-share offering. Since then, the program has grown to a fleet of 5,824 bicycles that are geotracked and locked into a network of 692 stations across Chicago. The bikes can be unlocked from one station and returned to any other station in the system anytime.

Until now, Cyclistic’s marketing strategy relied on building general awareness and appealing to broad consumer segments. One approach that helped make these things possible was the flexibility of its pricing plans: single-ride passes, full-day passes, and annual memberships. Customers who purchase single-ride or full-day passes are referred to as casual riders. Customers who purchase annual memberships are Cyclistic members.

Cyclistic’s finance analysts have concluded that annual members are much more profitable than casual riders. Although the pricing flexibility helps Cyclistic attract more customers, Moreno believes that maximizing the number of annual members will be key to future growth. Rather than creating a marketing campaign that targets all-new customers, Moreno believes there is a solid opportunity to convert casual riders into members. She notes that casual riders are already aware of the Cyclistic program and have chosen Cyclistic for their mobility needs.

Moreno has set a clear goal: Design marketing strategies aimed at converting casual riders into annual members. In order to do that, however, the team needs to better understand how annual members and casual riders differ, why casual riders would buy a membership, and how digital media could affect their marketing tactics. Moreno and her team are interested in analyzing the Cyclistic historical bike trip data to identify trends.

### Deliverables:

1. A clear statement of the business task
2. A description of all data sources used
3. Documentation of any cleaning or manipulation of data
4. A summary of your analysis
5. Supporting visualizations and key findings
6. Your top three recommendations based on your analysis

# Analysis Phases

## Ask phase

Three questions will guide the future marketing program:

1. **How do annual members and casual riders use Cyclistic bikes differently?** This question aims to uncover the usage patterns and preferences between annual members and casual riders. Understanding differences in usage frequency, trip duration, popular routes, and bike types can provide insights into the unique needs of each group.

2. **Why would casual riders buy Cyclistic annual memberships?** Exploring the motivations behind casual riders transitioning to annual memberships is crucial for designing effective marketing strategies. Identifying the factors that incentivize casual riders to commit to long-term memberships can inform targeted messaging and promotional efforts.

3. **How can Cyclistic use digital media to influence casual riders to become members?** Understanding the role of digital media in influencing consumer behavior can help Cyclistic optimize its marketing channels. Analyzing engagement metrics, conversion rates, and user demographics across digital platforms can provide valuable insights into effective messaging and outreach strategies.

**Analysis Objectives:**

Identify usage patterns and preferences between annual members and casual riders.
Uncover key motivations driving casual riders to purchase annual memberships.
Determine the effectiveness of digital media channels in converting casual riders into annual members.

The question for this analisys is: **How do annual members and occasional riders differ in their use of Cyclistic bikes?****

## What is the problem I'm trying to solve?

The problem at hand is understanding the differences in usage patterns between annual members and casual riders of Cyclistic bikes. By uncovering these distinctions, we aim to develop targeted marketing strategies to convert casual riders into annual members, ultimately maximizing the number of annual memberships and fostering future growth for Cyclistic.

## How can your insights drive business decisions?

Insights derived from analyzing the usage patterns of annual members and casual riders will enable Cyclistic to make informed decisions regarding marketing strategies, resource allocation, and customer engagement initiatives. By understanding the behaviors and preferences of each customer segment, Cyclistic can tailor its marketing efforts to effectively target casual riders and encourage them to transition into annual members.

## Identify the business task

The business task is to analyze the usage patterns of Cyclistic bikes among annual members and casual riders to identify differences and trends. This analysis will inform the development of targeted marketing strategies aimed at converting casual riders into annual members, aligning with Cyclistic's goal of maximizing annual memberships for future growth.

## Consider key stakeholders

The key stakeholders involved in this task include:

- Lily Moreno, Director of Marketing: Responsible for overseeing the development and implementation of marketing strategies.
- Cyclistic Marketing Analytics Team: Responsible for collecting, analyzing, and reporting data to guide marketing strategy.
- Cyclistic Executive Team: Responsible for approving recommended marketing programs and strategic initiatives.

## A clear statement of the business task

Analyze the usage patterns of Cyclistic bikes among annual members and casual riders to identify differences and trends, with the goal of developing targeted marketing strategies aimed at converting casual riders into annual members.

## Prepare Phase

In the Prepare phase, we focus on gathering and cleaning the data necessary to address the key questions identified in the Ask phase. This phase involves understanding the data structure, handling missing values, and ensuring data integrity for accurate analysis.

I have used Cyclistic's historical trip data to analyze and identify trends. Download cyclist trip data for the last 12 months. This data is public and can be used to explore how different types of customers use bicycles.

Please note that data privacy concerns prohibit the use of personally identifiable passenger information. This means that pass purchases are not connected to credit card numbers to determine if occasional riders live in the bicycle service area or if they have purchased multiple individual passes.

## Where is your data located?

The data used for the analysis are held in a public repository, they can be found [here](https://divvybikes.com/system-data). These data are provided in accordance with the [Divvy data license agreement](https://divvybikes.com/data-license-agreement) and are published monthly.

## How is the data organized?

Each trip is anonymized and includes:

- Trip start day and time
- Trip end day and time
- Trip start station
- Trip end station
- Rider type (Member, Single Ride, and Day Pass)

The data has been processed to remove trips that are taken by staff as they service and inspect the system; and any trips that were below 60 seconds in length (potentially false starts or users trying to re-dock a bike to ensure it was secure).

## Are there issues with bias or credibility in this data? Does the data ROCCC?

Let's check if this data set is reliable, original, complete, current and cited.

- The data source is reliable because it is data that has been previously processed to eliminate inconsistencies or short trips that could cause credibility problems in the analysis.

- The source of the data is original because it has been possible to locate the original source of the data without resorting to third-party information.

- The data source is complete with respect to its columns, however, in some months the information is incomplete, there are null or empty values that can cause problems in the analysis.

- The data source is updated. The documentation and repository containing the data sets is updated monthly and periodically, giving you assurance that it is the most up-to-date information available.

- Finally, the source has been cited and verified since its main purpose is to serve as a source of information for a case study.

## How are you addressing licensing, privacy, security, and accessibility?

Licensing: The agreement establishes a non-exclusive, royalty-free, limited, perpetual license for users to access, reproduce, analyze, copy, modify, distribute, and use the Divvy system data for lawful purposes.

Privacy and Security: Users are prohibited from using the data in unlawful manners or attempting to correlate it with identifiable information of customers or members of Bikeshare. They are also restricted from circumventing access restrictions or using data mining methods.

Accessibility: The data is made available to the public, subject to the terms and conditions of the agreement, implying an accessibility aspect.

Ownership: The City of Chicago owns all right, title, and interest in the data. Bikeshare may modify or cease providing the data at any time, without notice, at its sole discretion.

## How did you verify the data’s integrity?

I have been able to verify the integrity of the data by performing the following validations:

- **Visual check**: downloading, unzipping and seeing if the CSV files are complete and correctly formatted. This has allowed me to identify problems such as missing data and null values.

- **Size Check**: I have verified that the size of the files is significant. And I have noticed that CSV files with incomplete data have abnormally small file sizes.

- **Record comparison**: I have been able to observe that the CSV files have the expected format and generally contain the same data. I uploaded the dataset to Kaggle, which allowed me to quickly identify data and outliers using Kaggle's visualization tools.

- **Checking Headers and Data Types**: I have ensured that the column headers are consistent across all files and that the column data types are as expected.

## How does it help you answer your question?

**Trip Start and End Day/Time:**

These timestamps allow us to analyze usage patterns, such as peak hours and days, for both annual members and casual riders. Understanding when riders are most active can help tailor marketing campaigns and promotions accordingly.

**Trip Start and End Station:**

Station data enables us to analyze popular routes, station utilization rates, and trip durations. Identifying frequently used stations and common trip destinations provides insights into rider behavior and preferences.

**Rider Type (Member, Single Ride, and Day Pass):**

Categorizing riders into different types allows us to distinguish between annual members and casual riders. Analyzing the distribution of rider types, trip frequencies, and duration can help identify trends and patterns specific to each group.

## Are there any problems with the data?

Some files may contain null or empty values, which need to be addressed during data preprocessing. Techniques such as imputation or removal of incomplete records may be necessary to ensure data quality and integrity.

## Process Phase

- In the processing phase, the data sets were stored in csv format in Kaggle.
- Subsequently, all these files were read and a single dataframe was created using the pandas and glob libraries.

  - glob: library used to search for files that match certain naming patterns in a file system. It allows to automate the identification and loading of files.
  - pandas: allows data reading and writing, cleaning, transformation, statistical and aggregation operations, index and column manipulation, filtering, data selection and visualization.

- Several columns have been identified as having null or empty values. Missing values are found in the following columns.

  - start_station_name
  - start_station_id
  - end_station_name
  - end_station_id
  - end_lat
  - end_lng

- Columns with null or empty values have been removed.
- In addition, duplicate rows have been searched for, however, no rows with repeated values have been found.
- Let's analyze time trends, we need to change the type of the date columns to a date-time object
- We can separate the date (in differents columns) for a better analysis, the new columns are:

  - ride_length: ride duration (ended_at - started_at)
  - day_of_week: Monday, Tuesday, ...
  - month: Name of the month, taken from started_at
  - ride_start_hour: Hour taken from started_at (ex. 15, 13, 19, ...)
  - ride_length_days: ride duration in days
  - ride_length_minutes: ride duration in minutes

- Finally, records with a negative duration have been eliminated to avoid conflicts in the analysis.

## Analyze Phase

In this pass, important statistical data and calculations have been obtained for the analysis:

-  Calculate the average ride_length_minutes by membership

| Membership | Average Ride Length mins |
|--------|------------|
| casual | 28.25 mins |
| member | 12.53 mins |


-  Calculate the median ride_length_minutes by membership

| Membership | Median Ride Length mins |
|--------|------------|
| casual | 11.85 mins |
| member | 8.52 mins |


-  Calculate the average ride_length_minutes by membership by day_of_week

| Membership  | Day of week | Average Ride Length mins |
|--------|----------|-------|
| casual | Friday   | 27.26 mins |
|        | Monday   | 27.71 mins |
|        | Saturday | 32.14 mins |
|        | Sunday | 32.86 mins |
|        | Thursday | 24.73 mins |
|        | Tuesday | 25.08 mins |
|        | Wednesday | 24.30 mins |
| member | Friday   | 12.48 mins |
|        | Monday   | 11.90 mins |
|        | Saturday | 13.94 mins |
|        | Sunday | 13.99 mins |
|        | Thursday | 12.02 mins |
|        | Tuesday | 12.01 mins |
|        | Wednesday | 11.95 mins |

-  Calculate the max ride_length_minutes by membership

| Membership | Max Ride Length mins |
|--------|------------|
| casual | 98489.07 mins |
| member | 1559.67 mins |

-  Calculate the mode day_of_week: ´Saturday´

-   Calculate the number of rides by membership by day_of_week

| Membership  | Day of week | Total Rides |
|--------|----------|-------|
| casual | Friday   | 311907 |
|        | Monday   | 234818 |
|        | Saturday | 410684 |
|        | Sunday | 335668 |
|        | Thursday | 270596 |
|        | Tuesday | 246211 |
|        | Wednesday | 249153 |
| member | Friday   | 531582 |
|        | Monday   | 494558 |
|        | Saturday | 472846 |
|        | Sunday | 408829 |
|        | Thursday | 589572 |
|        | Tuesday | 576743 |
|        | Wednesday | 586438 |

-   Calculate the total rides by membership

| Membership | Total Rides |
|--------|------------|
| casual | 2059037 |
| member | 3660568 |

-   Calculate the total rides by membership by bike type

| Membership  | Bike Type | Total Rides |
|--------|----------|-------|
| casual | classic_bike   | 876858 |
|        | docked_bike   | 78287 |
|        | electric_bike | 1103892 |
| member | classic_bike   | 1819110 |
|        | electric_bike   | 1841458 |

## Share Phase

### Were you able to answer the question of how annual members and casual riders use Cyclistic bikes differently?

Yes, the data provides insights into the differences between annual members and casual riders in terms of ride length, day of the week usage patterns, and bike type preferences. Casual riders tend to have longer average and median ride lengths compared to annual members, and they predominantly use electric bikes. Annual members, on the other hand, have shorter ride lengths and prefer classic bikes.

### What story does your data tell?

The data reveals distinct usage patterns and preferences between annual members and casual riders. It suggests that casual riders may use Cyclistic bikes more for leisure or longer trips, while annual members may use them for shorter, more frequent trips, possibly for commuting or everyday activities.

### How do your findings relate to your original question?

The findings provide valuable insights into the behavior and preferences of Cyclistic's customer segments, which directly addresses the original question of understanding how annual members and casual riders use the bikes differently. These insights can inform targeted marketing strategies aimed at converting casual riders into annual members.

### Who is your audience? What is the best way to communicate with them?

The audience includes Cyclistic's marketing team, executives, and stakeholders involved in decision-making processes. Communicating findings through concise reports, presentations, and interactive visualizations can effectively convey the insights and recommendations to different stakeholders.

### Can data visualization help you share your findings?

Absolutely, data visualization can be instrumental in presenting key findings in a clear, engaging manner. Visualizations such as bar charts, pie charts, line graphs, and heatmaps can effectively illustrate trends, comparisons, and distributions in the data.

> The generated visualizations can be viewed in the attached Jupiter notebook or at [this kaggle link](https://www.kaggle.com/code/bryana/cyclistic-bike-share-analysis).

## Act Phase

Based on the analysis of Cyclistic's bike trip data, it is evident that there are notable differences in the behavior and preferences of annual members and casual riders. Casual riders tend to engage in longer trips, primarily on weekends, and prefer electric bikes. Annual members, on the other hand, opt for shorter trips, frequently utilize classic bikes, and exhibit more consistent usage patterns throughout the week.

The company can attract casual riders to become members by offering discounts on weekends, as casual riders tend to prefer riding during this time. Since casual riders often ride for longer durations, the company should also consider implementing flexible pricing for extended rides among those who become members. While member riders maintain consistency throughout the year, casual riders show a preference for the summer season. Therefore, the company should focus on improved marketing strategies and flexible pricing options during the summer to encourage casual riders to transition into members. Initiating a marketing campaign highlighting the advantages of membership during the summer, weekends, and for longer rides could effectively promote this transition.

On average, casual users take longer trips, lasting about 28 minutes, compared to members who take trips averaging 12 minutes. Casual users' trip lengths vary greatly throughout the week, peaking on weekends, while members consistently take trips of similar lengths, suggesting they are regular routines. Member users primarily use the service to commute to and from work, as indicated by peaks in usage at 8am and 6pm, which are not observed among casual users or on weekends.

### Recommendations:

##### Targeted Marketing Campaigns:

- Develop targeted marketing campaigns aimed at converting casual riders into annual members. Highlight the benefits of annual memberships, such as convenience, cost savings, and access to a wider range of bike options. Tailor messaging to address the specific needs and preferences of casual riders, emphasizing the value proposition of becoming a Cyclistic member.
- A better analysis is possible if data are collected correctly for columns such as (start_station_name, start_station_id, end_station_name, end_station_id). This data would provide accurate information about the locations where users make the most or least amount of bike trips and you can create marketing campaigns targeted to those specific locations or even consider opening new stations and closing others.
- Make a summer promotion; lower price only available in summer. Make a weekend member program. Special weekend like special price only for member.

#### Promotional Offers and Incentives:

- Offer promotional discounts or incentives to encourage casual riders to sign up for annual memberships. Consider limited-time offers, referral programs, or exclusive benefits for new members to incentivize conversion. Utilize digital media channels to promote these offers and engage with potential members effectively.
- A loyalty program can be introduced where occasional yet regular users have the opportunity to exchange their accumulated points for a membership package at a reduced price.

#### Enhanced Rider Experience:

Focus on enhancing the overall rider experience for both annual members and casual riders. This could involve improving bike availability, optimizing station locations, and introducing additional features or services that cater to diverse user needs. By prioritizing customer satisfaction and convenience, Cyclistic can attract and retain more members over time.


Next Steps:

- Implement the recommended marketing strategies and promotional campaigns based on the insights gathered from the analysis.
- Monitor and track the effectiveness of the initiatives through key performance indicators (KPIs) such as membership sign-ups, conversion rates, and rider feedback.
- Continuously analyze customer feedback and usage data to identify opportunities for further optimization and refinement of marketing efforts.

---

Exploring additional data sources such as customer surveys, demographic information, and user feedback could provide deeper insights into the motivations and preferences of Cyclistic's customer base. Incorporating qualitative data alongside quantitative analysis can offer a more comprehensive understanding of customer behavior and inform future decision-making processes.

## Built with

- Python
- Pandas
- Matplotlib
- Jupyter Notebook
- Seaborn

## Stay in touch

- Website - [www.bryan-aguilar.com](https://www.bryan-aguilar.com/)
- Medium - [baguilar6174](https://baguilar6174.medium.com/)
- LinkeIn - [baguilar6174](https://www.linkedin.com/in/baguilar6174)
