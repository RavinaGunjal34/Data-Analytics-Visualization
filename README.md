# Data-Analytics-Visualization
This an Internship on Forage at Accenture - North America

Introduction:

I participated in Accenture North America's data analytics virtual internship via Forage in a bid to use my data analytics skill to solve real-world problems, it was an overall thrilling experience for me and I’ll be sharing the wholesome experience with you in this article. About forage, forage is an open-access platform designed to unlock exciting careers for students by connecting them with company-endorsed Virtual Work Experience Programs. 

The internship program was subdivided into sections, each section had a series of tasks to be completed. Beginning with project understanding.

Section 1:Project Understanding

This section was keen on establishing facts about the tasks ahead and outlining the project deliverables. For the internship, I worked as a Data Analyst at Accenture within a larger team, where each member has a different role and level of responsibility. My team was assigned a new project for a client called Social Buzz. I got the project brief and it was my responsibility to Understand the client and business problem at hand, identify the requirements that need to be delivered for this project and identify which tasks I should focus on as a Data Analyst.

ABOUT THE CLIENT

Social buzz is a fast-growing technology company that emphasizes content by keeping all users anonymous, only tracking user reactions to every piece of content. Over the past 5 years, Social Buzz has reached over 500 million active users each month. They have scaled quicker than anticipated and need the help of an advisory firm to oversee their scaling process effectively. To start our engagement with the client, Accenture has begun a 3-month initial project to prove to them that we are the best firm to work with. During this period Social Buzz expects the following from Accenture:

·       An audit of their big data practice

·       Recommendations for a successful IPO

·       An analysis of their content categories that highlight the top 5 categories with the largest aggregate popularity

As the data analyst, an analysis of their content categories that highlight the top 5 categories with the largest aggregate popularity is the task most relevant to me. In this section, I practised project planning and strategy. Let's dive into the next step, shall we?

Section 2: Data cleaning and Modelling

Now I have a good understanding of the project and my role, it’s time to get to work. The client has sent over a data model and 7 data sets each stored in a CSV file, each data set contains different columns and values. The data model shows the relationships between all of the data sets, as well as any links that can be used to merge tables. To complete this section I did the following:

2.1 Requirements gathering: Here I used the data model to identify which datasets will be required to answer the business question which is to figure out the top 5 categories with the largest popularity. After going through the data model I identified 3 data sets that contained the data relevant to the business question. The data set names are Reaction, Content, and Reaction Types.

No alt text provided for this image
Data Model
My thought process leading to the aforementioned selection:

·       The brief carefully states that the client wanted to see “An analysis of their content categories showing the top 5 categories with the largest popularity”.

·       The data model explains that popularity is quantified by the “Score” given to each reaction type. Therefore, I need data showing the content ID, category, content type, reaction type, and reaction score.

·       So, to figure out popularity, I’ll have to add up which content categories have the largest score.

2.2 Data Cleaning: The content data set had 1001 rows and 5 columns namely content ID, user ID, type, category, and URL. Thereaction data set on the other hand had 24,573 rows and 4 columns namely content ID, user ID, reaction type, and datetime. While the reaction type data set had 15 rows and 3 columns namely reaction type, sentiment and score. In addition, all 3 data sets had an additional nameless column containing numbers in ascending order.

No alt text provided for this image
Content, Reactions and Reaction type CSV files before cleaning

To clean the data sets I employed the following:

·       Removal of irrelevant columns: I deleted the user ID, URL, and the nameless columns from their respective data sets because they are irrelevant to the task at hand.

·       Changing data types: I changed the data type of some values within a column to their corresponding data type.

2.3 Data modelling: 

The focus here is to figure out the top 5 content categories. To complete the data modelling process, I followed these steps:

·       I created a final data set by merging the three tables using the Vlookup function in excel, to do this I used the Reaction table as the base table, and then I joined the relevant columns from the Content data set, using a common unique identifier which was the content ID column, I then joined the Reaction types data set to the merged data set using the reaction type column which serves as the common unique identifier. After which I proceeded to create a full outer join. After this, I deleted the repeated columns. The result of this process is a single dataset with 7 columns and 24,573 rows.

Let the analysis begin!

·       Analysed the data to get the top 5 performing categories: To do this I used the ‘SUMIF’ function in Excel to aggregate the sum of each unique category. I used the formula below to achieve this. The cell ‘E912’ contains the unique category Animals, to get the sum of the other categories, I replaced the cell number with the cell number of other content categories to get their respective sum. I proceeded to sort the results in descending other to get the top 5 categories.
By completing this section, I practised data modelling and data understanding skills.

Section 3: Data Visualization and Storytelling

This phase is focused on bringing the data to life, as a data analyst my job is to connect the business and the data. After uncovering insights from the data, I needed to communicate the relevant insights in a way that is clear, concise and engaging to my client and team members. This requires creating data visualizations and a PowerPoint presentation for Social Buzz that reports on their content performance. I created this dashboard using Tableau to analyse the top 5 categories, unique categories and the number of posts per month, popular category by reaction type. I then used the data generated to create a graph.

Summary:

We tackled this task and found the top 5 most popular categories as asked, but we also went one step further. 

- We found that animals and science are the two most popular categories, suggesting that users like "real-life" and "factual" content.

- We also found that food was a common theme amongst popular content and the most popular food category was healthy eating. This could be a signal to show the types of people that are using your platform, and you could use this insight to boost engagement even further. For example, you could run a campaign with content focused on this category or work with healthy eating brands to promote content. 

- As much as this analysis was insightful, we are ready to take it to the next stage and we have the expertise within Accenture to help you realize these kinds of insights in production across your organization and in real-time. We would love to help you with this.
