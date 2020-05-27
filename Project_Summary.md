## Purpose of the Project
The purpose of this project was to use data collected from the point of sales (POS) of a small start-up in Portland, OR in order to gain business insights the company can use for future growth. The areas explored include sales, store sections, products, and items. This report captures the questions explored and analyses performed using Excel. 

This project looks at the data for just under the first two years of the company's life. Analysis will provide insight on what actions the company should take around product curation and store sections moving forward. 


## KPIs
* Sales per Square Feet
* Year-Over-Year (YOY) Growth
* Gross Profit vs Net Profit


## Objectives

#### 1. Understand the scope of the data
* How many and which months and years has the company been operating? Which of those provide enough data to address the other objectives of the project?
* How are the sections of the store classified? 
* How do the tables of data analyzed relate to one another?
* What other information is important to understand about the store to gain insight from the data and analysis?

#### 2. Sales
* What is the Year-Over-Year (YOY) Growth of the company?
* What hours of the day are sales the highest and what insight does this provide for staffing? Which hours are most likely to be best for focus time?
* What months should the business focus on advertising and other additional optional costs? (1A)

#### 3. Tag (Section)
* What sections of the store should the business focus on so revenue can increase without having costs increase, thereby leading to larger profit margins?
* How did changing the store layout affect sales for each section of the store, paying specific attention to the Organization section?
* What are the Sales per Square Feet for each section?

#### 4. Product
* What specific products should the business focus on so revenue can increase without having costs increase, thereby leading to larger profit margins?
* How should the business approach product display for different days of the week? (2A)
* ((Products by month?))

#### 5. Item
* Which sections are overcrowded with items and which should the business focus on to curate the best choices for customers?
* What is the ideal number of items per section to return the best profit margin?
* Which section can the business expect to have the highest number of visitors and thereby accomodate with appropriate square footage?
* How can the business maximize inventory storage and plan an appropriate amount of space for each section?


## Analysis
#### Objective 1. Data Details
The data dictionary provides information on the database including the contents, structure, format and relationship of the elements to aid in understanding the data. Below is the data dictionary for this project:

![](future image link here)

* The data dictionary shows that although the data analyzed covers January 2018 - April 2020, not all months are important for analysis. Most analyses use data from June 2018 - February 2020, while sales analyses use data from June 2018 - April 2020. February 2018 - May 2018 are excluded as no sales were recorded those months.

* The main sections of the store are found under "Tag" (time management, motivation, focus, and organization). Other sections will be listed in the legend of the respective analysis.

Another helpful way to understand the data is with an Entity Relationship Diagram (ERD). An ERD shows how the tables (entities) in a database relate to one another. The following ERD was created using the Google Drive diagram editor, draw.io:

![](future image link here)

* The ERD demonstrates how the tables are related. The Product_SKU is used as a primary key to connect the Product, Weekly Revenue, Daily Revenue, and Monthly Item Count tables. Tag is used to connect the Weekly Item Count and Tag / Section tables and Hourly Sales stands alone for analyses.

* Other important considerations when reviewing the report:
  * Store hours were 10am - 6pm from __________; from _________, store hours were 11am - 6pm. Monthly workshops also provided one or more days a month where store hours extended to 8pm.
  * During the holidays in 2018, hours varied outside of those listed above. Also, revenue includes online sales which were not constricted to any specific timeframe.
  * The section listed as "blank" is a catch all for manually entered sales and therefore does not reflect an accurate gross profit as cost of good sold is not recorded.
  * 


#### Objective 2. Sales

* In order to calculate the Year-Over-Year growth of the company, June - December were taking into consideration for YOY growth between 2018 and 2019 as business began in June 2018. For YOY growth between 2019 and 2020, only January and February were examined as March and April numbers were negative due to COVID-19. YOY growth under these stipulations can be seen in the following image:

![YOY Growth](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/YOY_growth.png =100)

Due to the lack of consistency between months considered for each year, the growth numbers cannot be directly compared. When observing growth between specific months from year to year, June, July, and August show the highest growth numbers. This may be due to either seasonal shopping trends or overall growth from the companies inception. Monthly growth is displayed below:

![Monthly Growth](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Monthly_growth.png =100) 

-----
![2018 Hourly Chart](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Hourly_chart_2018.png =100) ![2019 Hourly Chart](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Hourly_chart_2019.png =100)  ![2020 Hourly Chart](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Hourly_chart_2020.png =100) 

* Considering morning sales, in 2018, highest sales varied between 12-2pm; in 2019, highest sales were from 12-1pm; in 2020, sales were trending toward 1-2pm being highest again. Considering evening sales, in 2018, sales slowly tapered off until close at 7pm; however, in 2019, sales saw an uptick from 5-6pm with a sharp drop due to a 6pm closing time; for 2020, the trend appeared as an uptick between 4-5pm. Sales may have continued to increase between 6-7pm in 2019 however, in 2020 it appears 
  * Staffing should reflect the trends above. Moving forward, if an increase in staffing is needed, overlap would best during early afternoon hours. Furthermore, when looking at trends between months, the following data from 2019 and 2020 demonstrates extra staffing for December, January, and fall evenings. Actual revenue numbers have been redacted but darker green indicates higher sales.
  ![2019 Hourly Table](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Hourly_table_2019.png =100) ![2020 Hourly Table](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Hourly_table_2020.png =100)
  * When thinking about ideal focus hours, fewer interruptions provide opportunity for better focus. Without the data for transactions per hour, revenue by hour provides an estimate for when transactions per hour were likely higher. In 2019, the best focus hours would have been between 3-5pm; in 2020, the best hour for focus seems to be trending toward 3:30-4:30pm.
  
-----
![2019 Gross Profit](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/gross_profit_2019.png =100)

* Based on 2019, March, August, and December would be the best months to focus on advertising campaigns or other extra expenses as these months brought in the highest profits. Advertising efforts may help drive up profits for months following these three. Additionally, this data can be used to prepare inventory for the aforementioned months as this is when sales are highest. 


#### Objective 3. Tag (Section)


#### Objective 4. Product



## Summary