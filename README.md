# Investigate_Business_Hotel_using_Data_Visualization
Investigate Business Hotel Using Data Visualization


# Background and Objective
It is crucial for a company to consistently analyze its business performance. In this instance, I will delve deeper into the hospitality industry. My focus is to understand the customer behavior in hotel reservations and its correlation with the cancellation rate. The insights gained will be presented in the form of data visualizations for better comprehension and enhanced persuasiveness

# Scope of problem
The objective is to analyze customer behavior in hotel reservations within the hospitality industry and investigate its correlation with the cancellation rate. Through data visualization, the aim is to provide comprehensive insights that enhance understanding and persuasiveness in assessing business performance within this sector.

# Data

# Data Preprocessing
1. Data containing null values will be filled with zeros, indicating:
- company: guests who are not affiliated with any company
- agent: guests who make reservations without going through an agent
- children: guests who do not bring any children
  
2. For the 'City' attribute, null values will be replaced with 'unknown' since the exact city is not known.
3. The features "Children," "Agent," and "Company" can be converted to integers, as their data appears to be representable with integer values.
4. Modify 'Undefined' in the 'meal' category to 'no meal' since it represents the same data.
5. Data without a unique_id/unique_booking_id and date may contain information resulting from the same reservation at different times.
6. The dataset sets Adults' value to 0, signifying it's impossible without adults. A newly engineered feature, stay_duration, sums stays_in_weekend_nights and stays_in_weekdays_nights to indicate total stay duration; instances with a duration of 0 are excluded. The adr (Average Daily Rate), derived from room revenue divided by rooms sold, contains negative values originating from sales data.

# Data Analysis
## Monthly Hotel Booking Analysis Based on Hotel Type

![image](https://github.com/pwirap/Investigate_Business_Hotel_using_Data_Visualization/assets/99533745/822528b4-730b-4d53-9afb-1922961af020)

1. Overall, City Hotels are generally more preferred than Resort Hotels.
2. Broadly speaking, Resort Hotels exhibit a more stable monthly booking average compared to City Hotels, which show significant variations during the Holiday Season.
3. There is an increase in the average booking rates during the High Demand months or holiday seasons in Indonesia, namely the mid-year period (May to July) and the year-end period (October to December).
4. Following the holiday season, a decline in average booking rates is observed for City Hotels.

## Impact Analysis of Stay Duration on Hotel Bookings Cancellation Rates

![image](https://github.com/pwirap/Investigate_Business_Hotel_using_Data_Visualization/assets/99533745/08a5b564-972c-4d1c-ad7e-8c16f7476360)

1. There is a positive correlation between the duration of stay and the cancellation rate for all types of hotels, with the most noticeable impact observed in City Hotels.
2. The longer the duration of stay, the higher the cancellation rate for hotel reservations.
3. In City Hotels, the highest cancellation rate is observed for stays exceeding one month, reaching 95%.
4. The cancellation rate is quite high, necessitating further analysis and a more specific examination of relationships to mitigate cancellations effectively.

## Impact Analysis of Lead Time on Hotel Bookings Cancellation Rate

![image](https://github.com/pwirap/Investigate_Business_Hotel_using_Data_Visualization/assets/99533745/affad078-9651-4e69-b73e-7fd8667a4ace)

1. The time interval between booking and arrival significantly influences the cancellation rate for each type of hotel.
2. A one-month lead time has the lowest cancellation rate, approximately 20% for each hotel.
3. The time interval of 10 months to over a year exhibits the highest cancellation rate.



