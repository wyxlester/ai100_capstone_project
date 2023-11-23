# HDB Resale Capstone Project

Hello, this is a data analytics project, comprising of data cleaning, data preparation and data visualisation activities. Data is extracted from Kaggle, this is also a capstone project for AI100 course with Heicoders Academy.

1. Background
Getting a HDB is probably one of the biggest financial decisions many Singaporeans have to make, given its exhorbitant cost. Making a wrong decision could set you back several years in terms of opportunity cost & time value of money. 
![image](https://github.com/wyxlester/ai100_capstone_project/assets/17344234/ecbe90ba-63bc-4cfc-92f7-13c12b6164ea)

In this project, we seek to build data visualisation to shed light on the HDB resale market, and provide key consideration parameters to help us make better decisions in choosing a:

(1) HDB Resale flat, or
(2) BTO flats that are likely to appreciate in the resale market


2. Loading the Dataset
CSV data of Singapore HDB listings (73320 rows × 14 columns) loaded into a nested list, hdb_resale_listings

3. Data Cleaning
Write a loop to iterate through the data to perform some cleaning. The data columns we will be cleaning are:
- floor_area_sqm (convert to float)
- remaining_lease (extract only the years & convert it to float)
- resale_price (convert to float)
- longitude (convert to float)
- latitude (convert to float)

4. Data Preparation & Visualisation
a. Calculate the Number of Resale Flats in Each Town
b. Visualise the Number of Resale Flats in Each Town
<img width="603" alt="Screenshot 2023-11-23 at 5 41 26 PM" src="https://github.com/wyxlester/ai100_capstone_project/assets/17344234/88f16295-4157-4544-a5f2-80c005d3f36d">

We observe that developing estates such as Sengkang, Punggol, and Woodlands tend to have a much higher volume of resale flats compared to mature estates such as Bishan and Marine Parade, which do not have as much land parcels available for development.

These difference in resale volume could be due to:

Young couples upgrading from their initial BTOs in nearby areas (more prevalent in areas such as Sengkang, Punggol, Woodlands)
Potential for housing appreciation in developing estates like Sengkang and Punggol due to new amenities being developed

c. Calculate the Total Sale Value in Each Town
d. Calculate the Average Resale Value in Each Town
e. Visualise the Average Resale Value in Each Town
<img width="639" alt="Screenshot 2023-11-23 at 5 43 07 PM" src="https://github.com/wyxlester/ai100_capstone_project/assets/17344234/8f844599-f98c-4999-a45a-78c51d3cd1dc">

HDB flats in central areas like Bukit Timah and Bishan have some of the highest resale values. The convenience of living in these areas also contribute to the huge demand of BTO flats there; getting a BTO in these areas is almost like striking the lottery!
One interesting observation is the surprisingly high resale value of Punggol flats relative to other towns. While some may have the impression that Punggol flats are inaccessible and not desirable, the average resale value tells a different story. Observe that Punggol's resale value is markedly higher than areas like Ang Mo Kio and Bedok. In addition, the average resale value of Punggol flats is not that far off from matured estates like Clementi, Tampines & Serangoon.
A potential follow-up visualisation would be a time-series analysis of the Punggol HDB resale values over the years, and one might discover significant capital appreciation opportunities for Punggol BTO owners in the resale market!

f. Is the Lease an Important Factor in the HDB Resale Price?
<img width="634" alt="Screenshot 2023-11-23 at 5 44 17 PM" src="https://github.com/wyxlester/ai100_capstone_project/assets/17344234/9b8613ac-fa97-4c1a-accf-b800ab204d5b">

This line plot illustrates a close correlation between the remaining lease period and the resale value of flats sold after 2017.
Another observation from this chart is that, BTO owners who sell their flats near the Minimum Occupancy Period (MOP), with about 90 years of lease remaining, are likely to gain maximum resale value out of on their subsidised flats!

g. How does Floor Area Correlate with Resale Price?
<img width="984" alt="Screenshot 2023-11-23 at 5 46 13 PM" src="https://github.com/wyxlester/ai100_capstone_project/assets/17344234/7984e70c-db58-4e09-843a-0b7f18d218db">

The scatterplot above shows that floor area is closely and positively correlated with HDB resale prices, with some variance that can likely be attributed to their locations (as investigated above). If you're looking for a large HDB flat, be prepared to pay!

h. Comparing Select 4 Room Flats in Singapore
<img width="629" alt="Screenshot 2023-11-23 at 5 47 09 PM" src="https://github.com/wyxlester/ai100_capstone_project/assets/17344234/c1f7f4b5-71d6-4f73-84bf-9f81db06ef31">

From the boxplot, we see that 4-room resale flats in Clementi tend to cost more and can have a huge variance in price. If you're on a very tight budget, a resale flat in Woodlands may be the optimal choice. 4-room resales flats in Punggol and Tampines have similar prices, so it would be helpful to zoom into Punggol & Tampines estates and compare the amenities available to specific flats and sub-areas in each town, in order to make a more informed decision.

i. Construct a Heatmap of all 4 room resale listings in Singapore
<img width="802" alt="Screenshot 2023-11-23 at 5 47 51 PM" src="https://github.com/wyxlester/ai100_capstone_project/assets/17344234/14ae36a3-d8d6-4ffc-b7b3-d8d4ca9f8ed8">

j. Construct a Folium Marker Cluster of all 4 room resale listings in Singapore
<img width="911" alt="Screenshot 2023-11-23 at 5 48 29 PM" src="https://github.com/wyxlester/ai100_capstone_project/assets/17344234/e89e5f44-a339-48be-8db8-ee0cf86bb2d5">











