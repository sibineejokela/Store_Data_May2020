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
* What months should the business focus on advertising and other additional optional costs?

#### 3. Tag (Section)
* What main sections of the store should the business focus on so revenue can increase without having costs increase, thereby leading to larger profit margins?
* What additional sections of the store should the business focus on so revenue can increase without having costs increase, thereby leading to larger profit margins?

#### 4. Product
* What specific products should the business focus in different sections so revenue can increase without having costs increase, thereby leading to larger profit margins?
* What products sell best on different days of the week? Which specific products sell best overall when not categorized by section?


## Analysis
### Objective 1. Data Details
The data dictionary provides information on the database including the contents, structure, format and relationship of the elements to aid in understanding the data. Below is the data dictionary for this project:

![Data Dictionary](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Data_Dictionary.png)

* The data analyzed covers January 2018 - April 2020, however, not all months are important for analysis. Most analyses use data from June 2018 - February 2020, while sales analyses use data from June 2018 - April 2020. February 2018 - May 2018 are excluded as no sales were recorded those months.

* The main sections of the store are found under "Tag" (time management, motivation, focus, and organization). Other sections will be listed in the legend of the respective analysis.

Another helpful way to understand the data is with an Entity Relationship Diagram (ERD). An ERD shows how the tables (entities) in a database relate to one another. The following ERD was created using the Google Drive diagram editor, draw.io:

![Entity Relationship Diagram](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/ERD.png)

* The ERD demonstrates how the tables are related. The Product_SKU is used as a primary key to connect the Product, Yearly Revenue, Weekday Revenue, and Monthly Item Count tables. The Monthly Tag Revenue and Hourly Revenue tables stand alone for analyses.

* Other important considerations when reviewing the report:
  * Store hours were 10am - 6pm until September 9th, 2019, after which store hours were 11am - 6pm. Monthly workshops also provided one or more days a month where store hours extended to 8pm. For most months these workshops fell on Wednesdays.
  * During the holidays in 2018, hours varied outside of those listed above. Also, revenue includes some online sales which were not constricted to any specific timeframe.
  * The Build-A-Notebook section of the store was excluded from most analysis due to inaccurate data records regarding profit and loss. The inaccuracies resulted from the way revenue was tracked within the BAN section. Specifically, losses were recorded for each packet that made up each notebook resulting in inaccurately high losses.


### Objective 2. Sales

#### YOY Sales Growth

* In order to calculate the Year-Over-Year growth of the company, June - December were taking into consideration for YOY growth between 2018 and 2019 as business began in June 2018. For YOY growth between 2019 and 2020, only January and February were examined as March and April numbers were negative due to COVID-19. YOY growth under these stipulations can be seen in the following image:

<!-- ![YOY Growth](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/YOY_growth.png) -->
<img src="https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/YOY_growth.png" width="325">

Due to the lack of consistency between months considered for each year, the growth numbers cannot be directly compared. When observing growth between specific months from year to year, June, July, and August show the highest growth numbers. This may be due to either seasonal shopping trends or overall growth from the company's inception. Monthly growth is displayed below:

<!-- ![Monthly Growth](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Monthly_growth.png) -->
<img src="https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Monthly_growth.png" width="375">

-----
#### Hourly Sales Data

![2018 Hourly Chart](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Hourly_chart_2018.png) ![2019 Hourly Chart](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Hourly_chart_2019.png)  ![2020 Hourly Chart](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Hourly_chart_2020.png)


* Considering morning sales, in 2018, highest sales varied between 12-2pm; in 2019, highest sales were from 12-1pm; in 2020, sales were trending toward 1-2pm being highest again. Considering evening sales, in 2018, sales slowly tapered off until close at 7pm; however, in 2019, sales saw an uptick from 5-6pm with a sharp drop due to a 6pm closing time; for 2020, the trend appeared as an uptick between 4-5pm. Sales may have continued to increase between 6-7pm in 2019, however, in 2020 it appears the second sales peak had concluded by closing time at 6pm. 
  * Staffing should reflect the trends above. Moving forward, if an increase in staffing is needed, overlap would best during early afternoon hours. Furthermore, when looking at trends between months, the following data from 2019 and 2020 demonstrates extra staffing for December, January, and fall evenings. Actual revenue numbers have been redacted to respect company privacy but darker green boxes indicate higher sales.
  <!-- ![2019 Hourly Table](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Hourly_table_2019.png) ![2020 Hourly Table](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Hourly_table_2020.png) -->
  <img src="https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Hourly_table_2019.png" width="648"> <img src="https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Hourly_table_2020.png" width="231">

  * When thinking about ideal focus hours, fewer interruptions provide opportunity for better focus. Without data for transactions per hour, revenue by hour provides an estimate for when transactions per hour were likely higher. In 2019, the best focus hours would have been between 3-5pm; in 2020, the best hour for focus is trending toward 3-4pm.
  
-----
#### Monthly Gross Profit and Revenue

<!-- ![2019 Gross Profit](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/gross_profit_2019.png) -->
<img src="https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/gross_profit_2019.png" width="700">

* Based on 2019, March, August, and December would be the best months to focus on advertising campaigns or other extra expenses as these months brought in the highest profits. Advertising efforts may help drive up profits for months following these three. Additionally, this data can be used to prepare inventory for the aforementioned months as this is when sales are highest. 


### Objective 3. Tag (Section)

#### Main Store Sections

* The four main sections of the store are Focus, Motivation, Organization and Time Management. Year-to-year and, for the most part, month-to-month, Time Mangement has been the most successful section of the store. Comparing the two charts below also shows that revenue return is high as the number of items sold is comparable to other sections yet the revenue is much higher. The more interesting section is the focus section. This number of items sold from this section is consistently fewer than other sections, however, the revenue returned in this section is as higher or higher than others. Therefore, the business should focus on sales in the Focus section to increase revenue with least cost increases. 

![Revenue in Main Store Sections](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Store_Sections_Rev.png)
![Items Sold in Main Store Sections](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Store_Sections_Items.png)

#### Additional Best Selling Sections

Other top sections for the store include Books, Cash Wrap, Desk Tools, Dot Journaling, Notebook/Bar, Plants and Travel. The charts below explore these sections but also include the four main sections from above for comparison purposes. Here, the travel section replicates the trends in the Focus and Time Management sections with a small number of items sold and high revenue. Therefore, another area the business could focus on for increased revenue is the Travel section.

![Revenue in Additional Sections](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Store_Sections_additional_Rev.png)
![Items Sold in Additional Sections](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Store_Sections_additional_Items.png)

The data above takes revenue into consideration, however, gross profit is the more important measure. Gross profit was not included in the above analysis due to the limitations of the data. Specifically, only the yearly aggregate of gross profit was available. However, the following scatter plot shows the correlation between revenue and gross profit margins, indicating that a higher revenue is also indicative of a higher gross profit.  

![Yearly Revenue vs Gross Profit by Sections 2019, 2020](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Store_Sections_Rev_vs_GP.png) 

NOTE: CYON much higher in the items sold; excluded due to improper revenue and profit measurements. 
NOTE: Specific products discussed below:

-----



### Objective 4. Product

#### Products by Section

* The top revenue earning sections from 2018 - 2020 can be seen in the treemap below. As echoed in the analysis above, the Time Management section is at the very top. However, this trend changes when only the top five products are considered instead of all products within the section. These differences are discussed below.

![Revenue by Section 2018-2020](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Store_Sections.png)

When only the top five products per section are considered, the top revenue earning sections change drastically. This means that the top five products from the plants section bring in more revenue than the top five products from the time management section (for example). In order to increase revenue, the company could focus on and highlight these top five products for each section. Futhermore, this data has implications for products selected for an online arena. Having fewer products available but products that are top revenue earners can help with curation for an online store. 

![Revenue by Section and Product 2018-2020](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Store_Sections_and_Products.png)

#### Products by Weekday

Since we lack complete data for the full years of 2018 and 2020, 2019 was used to get a snapshot for top revenue earning products by weekday. This data can be used to determine what items to feature both in-store and on digital marketing platforms. Additionally, this data can be used to curate mystery boxes to contain best selling products or determine when to hold sales and which products to include in these sales. 

Looking at specific items helps further explore these ideas. A few key observations are that Poketo Angie Weekender Bags and plants bring in most revenue Friday-Sunday, workshops sell in-person more on Wednesday, and goal-setting items are top revenue earners on Monday. The Nuuna Hot Hot Dot A5, The 90 Day Gratitude Journal, and Resilient Management are other products that are top revenue earners for multiple days of the week. These three products would be good items to feature both in-store and online. Smaller items to feature or add to mystery boxes include frixion pens and le pens. As previously mentioned, the MiGoals Goals Journal and Goal Tracker Packs are top revenue earners on Mondays. The company may consider running a sale on goal-setting items on a Monday in the future.

![Top Ten Products for each Weekday 2019](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Products_Weekday.png)

When considering all days of the week together, the top ten revenue earning products in 2019 are as shown below. As previously mentioned, the Build-a-Notebook products were excluded from earlier analysis due to incorrect profit and sales data. It has been included here because isolated single products do not face the same flaws in the data as the BAN section does when considered as a whole. From this individual product analysis, one can see how well the $36 Build-a-Notebook sells as it is the second revenue earner when all days of the week are considered and is also in the top ten revenue earning product list every day (as shown above). 

<!-- ![Top Ten Products 2019](https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Products_All.png) -->
<img src="https://github.com/sibineejokela/Store_Data_May2020/blob/master/images/Products_All.png" width="600">

## Summary

The following insights are a quick snapshot of the discussion above:
* *Year-Over-Year growth* was **61% in 2019** (considering June - December) and **48% in 2020** (considering January - February)
* *Highest sales* occured between **12pm - 2pm** and again from **4pm - 6pm** with slight variation between years (2018 - 2020)
* Employees will be likely be least interrupted between 3pm - 4pm and therefore should plan *focus tasks* during this hour.
* Two areas the company could focus on to increase sales without huge increases in cost are the **Focus and Travel sections**
* Product analysis shows the *Time Management* section brings in the most revenue from all product sales. However, when considering only the top five products per section, the *Plants* section brings in the most revenue. These specific products can be found under Objective 4 above.
* The standard **Build-a-Notebook** offering was the *second highest revenue earning product* in 2019 (after general pens).

#### Recommended actions for the company moving forward are as follows:
* Double staff store 12 - 2 (+ fall evenings & winter holidays)
* Schedule focus 3 - 4
* Highlight products in the Focus and Travel sections. Starting with Manage Your Day-to-Day, The 90 Day Gratitude Journal, and Mindfulness on the Go Cards from the Focus section and Casio Watches and Habit Tracker Packs in the Travel section.
* Utilize the Top Ten Revenue Earning Sections based on the Top Five Revenue Earning Products treemap to curate online store items
* Use the Top Ten Revenue Earners (all days) to choose products to highlight