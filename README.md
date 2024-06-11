# Hotel Aggregator Analysis(E-Commerce)

## Data Cleaning

### Imported Data for Analysis: 

 - 	Number of columns: 75
 -  Number of rows: 23,185
 - 	Date range: 2009-2023 (with additional data for September 4th & 5th, 2023)
 - 	No duplicate values were identified.

### Cleaning Steps: 

 - 	Address Location Data: Split the host_location column into separate columns for host_city and host_country.
 - 	Clean Boolean Columns: Convert values in columns like host_is_superhost, host_has_profile_pic, host_identity_verified, has_availability, and instant_bookable from text 
    (e.g., "true", "false", "t", "f") to their corresponding boolean values (True/False).
 - 	Remove Unnecessary Columns: Delete irrelevant columns with missing data: neighbourhood_group_cleansed, calendar_updated, and bathrooms (containing only 2 entries).
 - 	License Removal: The license column was also removed, though the reason for its removal isn't mentioned in the original description.

### Output Data: 
The final dataset contains 72 cleaned columns.

## Insights

### 1.	Hotel Overview and Geographical Insight (2009-2013)
This analysis focuses on understanding the geographical distribution of hotel listings based on a dataset spanning 2009-2013 (10 years) with a total of 23,185 entries from two sources (city scrape: 16,551, previous scrape: 6,634).

**Distribution of Listings:** The data visualization reveals a significant concentration of listings in Melbourne and its suburbs, including Carlton, Collingwood, Docklands, 
  Doncaster, Elwood, and Fitzroy, each with over 100 listings. Melbourne stands out as the city with the highest number of listings, followed by Sydney. Overall, Australia 
  dominates the listings landscape with 16,199 properties, while the United Kingdom is a distant second with 106 listings. Despite the presence of listings in various 
  cities, Melbourne and its suburbs lead in terms of listing density.
  
**Missing Data:** A significant portion of listings lack city information (5,899) and country information (6,476). Further data cleaning is needed.

### Booking Availability:
**Instantly Bookable:** The majority of listings (17,255) allow instant booking, while 5,930 require additional confirmation.
### Seasonality:
**Upward Trend:** The line chart reveals a generally increasing trend in listings from 2010 to 2013, with a peak in August 2016.
•	Seasonal Dips: The data suggests consistent dips in listings during March and September, potentially indicating seasonal trends.
•	Geographical Concentration: The data indicates that Australia dominates the geographical landscape with 16,199 listings, while the United Kingdom follows with 106 listings. Other countries have fewer than 50 listings each.
2. Pricing and Availability Analysis
•	Pricing Trends: Entire rental unit have the highest total pricing, contributing over 2 million units, Entire home with 1,302,400, And others below 500,000. Private rooms and shared rooms have significantly lower total pricing.
•	Availability Trends: Listings show consistent availability throughout the year, with 365 days being the most common availability. The trend indicates an increase in property availability starting from October 2014, with August 2016 being the peak period for hosting. Seasonal dips are observed in March and September annually.
•	Top 10 property types are Entire rental unit, entire home, private room in home, private room in rental unit, Entire Condo, Entire town house, Entire serviced apartment, private room in town house, Entire guest house and Entire guest suit.
•	While entire homes and apartments dominate the listings with 16,887 while Private rooms come in a distant second with 5,932 listings.
3. Host Performance
Host Characteristics:
•	Superhost Status: The data reveals 5,621 Superhosts, 16,847 non-Superhosts, and 717 with missing status. Hosts responding within an hour tend to receive higher ratings, highlighting the importance of quick response times.
         To qualify for Superhost status, hosts must meet specific criteria, including: 
o	Hosting a certain number of nights or reservations per year.
o	Maintaining a high overall guest rating (typically above 4.8 stars).
o	Having a low cancellation rate.
o	Responding promptly to guest inquiries.
•	Response Times: Over 11,000 hosts respond within an hour, with more ratings compared to those with slower response times. 
•	Verification and Booking: Of the total hosts, 20,776 are verified, and 2,407 are unverified. Instant booking is available for 17,255 properties, whereas 5,930 properties do not offer this feature.
4. Review Scores and Guest Satisfaction
•	Review Analysis: Entire rental units receive the highest number of reviews, followed by entire homes and private rooms. The reviews cover various aspects such as accuracy, check-in, cleanliness, communication, location, and value. Review scores show a positive trend initially, with a dip between 2020 and 2022, followed by an upward trend until 2023.
•	Guest Satisfaction: The analysis of review categories indicates that guests generally favor entire rental units. However, there are areas for improvement in cleanliness and check-in processes.
•	Review Trends: While initially positive across all property types (entire rental unit having the highest), there was a dip from 2020-2022, followed by an upward trend until 2023.
5. Property Type and Room Analysis
•	Property Distribution: The majority of properties are entire homes/apartments (16,887), followed by private rooms (5,932), shared rooms (277), and hotel rooms (89).
•	Accommodation Trends: Entire rental units and entire homes are the most popular property types, showing higher demand and reviews compared to other types.
Limitations
•	Incomplete Data: There are significant gaps in the data, with 5,899 properties missing city information and 6,476 properties lacking country information. This limits the accuracy of geographical analysis.
•	Lack of Customer Data: The dataset does not include information about customer locations or their travel preferences, which restricts the ability to analyze customer behavior and preferences.
•	Temporal Gaps: The dataset spans from 2009 to 2013, with a notable dip in data quality and quantity from 2020 to 2022, potentially affecting the analysis of trends during these years.
Recommendations
•	Data Completion: Efforts should be made to fill in the missing city and country data to enhance the accuracy and completeness of the geographical analysis.
•	Investigate August Peak: The reason behind the peak in listings in August 2016 should be investigated to understand what factors contributed to this surge and how they can be leveraged in the future.
•	Seasonal Trends: The recurring dips in March and September should be examined to understand potential causes, such as seasonal travel patterns or market dynamics, and to develop strategies to mitigate these effects.
•	Enhanced Customer Insights: Future data collection should include information about customer locations and preferences to enable a more comprehensive analysis of customer behavior and improve marketing strategies accordingly.
