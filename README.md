# Cyclistic bike-share Analysis Case Study

This case study is about a fictitious company, Cyclistic. Where I will answer business questions, following the steps of the data analysis process: Ask, Prepare, Process, Analyze, Share and Act.

## Scenario

Cyclistic's marketing director believes that the company's future success depends on maximizing the number of annual members. Therefore, his team wants to understand how casual users and annual members use Cyclistic's bikes differently. From this information, his team will design a new marketing strategy to convert occasional riders into annual members. But first, Cyclistic executives must approve their recommendations, so they must be backed by compelling data and professional data visualizations.

## Characters and teams

- **Cyclistic**: A bike-share program that features more than 5,800 bicycles and 600 docking stations. Cyclistic sets itself apart by also offering reclining bikes, hand tricycles, and cargo bikes, making bike-share more inclusive to people with disabilities and riders who can’t use a standard two-wheeled bike. The majority of riders opt for traditional bikes; about 8% of riders use the assistive options. Cyclistic users are more likely to ride for leisure, but about 30% use the bikes to commute to work each day.

- **Lily Moreno**: The director of marketing and your manager. Moreno is responsible for the development of campaigns and initiatives to promote the bike-share program.ç These may include email, social media, and other channels.

- **Cyclistic marketing analytics team**: A team of data analysts who are responsible for collecting, analyzing, and reporting data that helps guide Cyclistic marketing strategy. You joined this team six months ago and have been busy learning about Cyclistic’s mission and business goals—as well as how you, as a junior data analyst, can help Cyclistic achieve them.

- **Cyclistic executive team**: The notoriously detail-oriented executive team will decide whether to approve the recommended marketing program.

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

## Ask phase

In the Ask phase, we define the key questions that will guide our analysis and help us understand the behavior of Cyclistic's customers.

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

# Process Phase

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
  - day_of_week_as_number: 0, 1, 2, ...
  - quarter:
  - day_of_month: Day of the month taken from started_at
  - month: Name of the month, taken from started_at
  - started_time: hour and minutes, taken from started_at
  - ended_time: hour and minutes, taken from ended_time
  - weekday_or_weekend: Identify if the day is a week day or a weekend

# Analyze Phase

...
