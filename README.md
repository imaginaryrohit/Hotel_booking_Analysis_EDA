# Hotel_booking_Analysis_EDA

## Description
We have been provided a dataset of the hotel industry of the region in which our startup aims to begin its initial operations. Our primary goal is to understand the market of this particular region and try to use our data analysis techniques to draw out key features of the market. Our secondary goal is to draw out actionable insights from our analysis and give conclusions about key aspects of the market such as cancellation rate, distribution channels, and alike Based upon the initial assessment we found that the data was pretty much clean except for some missing values in a few columns. Upon using the info() method, we draw out the following key insights about the data The dataset has a shape of (119390, 32) which means that it contains approximately 1.2 lakh rows and 32 columns. Our Dataset has 4 columns with float64 dtype, 16 columns with int64 dtype, and 12 columns with object dtype.In our Dataset, we observed null values in the following columns, null values in the children column, 488 null values in the country column, 16,340 null values in the agent column 112,593 null values in the company column.

# Objectives
The main objective is to explore the given dataset and discover the factors which govern the bookings. The dataset will be analyzed and from the conclusions drawn from it will be used to recognize the missteps taken by the manager. With this information, hotels will be equipped to improve their performance.

# Problem Statement
Data analysis is performed to answer the following questions:

### Some straight forward questions
1. Which agent makes most no. of bookings?
2. Which room type is in most demand and which room type generate highest adr?
3.  From which countries most of the customers visit these hotels?

### Hotel Wise Analysis
1. What is percentage of bookings in each hotel?
2. which hotel seems to make more revenue?
3. Which hotel has higher lead time?
4. What is preferred stay in each hotel?
5. Which hotel has longer waiting time?
6. Which hotel has higher bookings cancellation rate?
7. Which hotel has high chance that its customer will return for another stay?
### Distribution Channel wise Analysis
1. Which is the most common channel for booking hotels?
2. Which channel is mostly used for early booking of hotels?
3. Which channel has longer average waiting time?
4. Which distribution channel brings better revenue generating deals for hotels?
### Booking cancellation Analysis
1. Which significant distribution channel has highest cancellation percentage?
2. What causes the cancelation of bookings of rooms by customers?
### Time wise analysis
1. which month results in high revenue?
2. What is the booking %age of single, couple and family/friends?
3. How long do people stay at the hotels?

# Dataset
We are given a hotel bookings dataset. This dataset contains booking information for a city hotel and a resort hotel. It contains the following features.
- hotel: Name of hotel ( City or Resort)
- is_canceled: Whether the booking is canceled or not (0 for no canceled and 1 for canceled)
- lead_time: time (in days) between booking transaction and actual arrival.
- arrival_date_year: Year of arrival
- arrival_date_month: month of arrival
- arrival_date_week_number: week number of arrival date.
- arrival_date_day_of_month: Day of month of arrival date
- stays_in_weekend_nights: No. of weekend nights spent in a hotel
- stays_in_week_nights: No. of weeknights spent in a hotel
- adults: No. of adults in single booking record.
- children: No. of children in single booking record.
- babies: No. of babies in single booking record. 
- meal: Type of meal chosen 
- country: Country of origin of customers (as mentioned by them)
- market_segment: What segment via booking was made and for what purpose.
- distribution_channel: Via which medium booking was made.
- is_repeated_guest: Whether the customer has made any booking before(0 for No and 1 for Yes)
- previous_cancellations: No. of previous canceled bookings.
- previous_bookings_not_canceled: No. of previous non-canceled bookings.
- reserved_room_type: Room type reserved by a customer.
- assigned_room_type: Room type assigned to the customer.
- booking_changes: No. of booking changes done by customers
- deposit_type: Type of deposit at the time of making a booking (No deposit/ Refundable/ No refund)
- agent: Id of agent for booking
- company: Id of the company making a booking
- days_in_waiting_list: No. of days on waiting list.
- customer_type: Type of customer(Transient, Group, etc.)
- adr: Average Daily rate.
- required_car_parking_spaces: No. of car parking asked in booking
- total_of_special_requests: total no. of special request.
- reservation_status: Whether a customer has checked out or canceled,or not showed 
- reservation_status_date: Date of making reservation status.

# Data Preparation
- Remove duplicate rows
- Handling missing values.
- Convert columns to appropriate datatypes.
- Adding important columns

# Exploratory Data Analysis
EDA was carried out in 3 steps:

1. Correlation Analysis

It is used to measure the strength of the linear relationship between two variables and compute their association. Correlation analysis calculates the level of change in one variable due to the change in the other. Correlation analysis of the dataset was carried out using a correlation heatmap with the features.

2. Univariate Analysis

Uni means one and variate means variable, so in univariate analysis, there is only one dependable variable. The objective of univariate analysis is to derive the data, define and summarize it, and analyze the pattern present in it. In a dataset, it explores each variable separately.

3. Bivariate Analysis

Bi means two and variate means variable, so here there are two variables. The analysis is related to cause and the relationship between the two variables. 

# Conclusion
1. 61.1% bookings are for City hotel and 38.9% bookings are for Resort hotel
2. Avg adr of Resort hotel is slightly lower than that of City hotel. Hence, City hotel seems to be making slightly more revenue.
3. City hotel has slightly higher median lead time.
4. Most common stay length is less than 4 days and generally people prefer City hotel for short stay, but for long stays, Resort Hotel is preferred.
5. City hotel has significantly longer waiting time, hence City Hotel is much busier than Resort Hotel.
6. Almost 30 % of City Hotel bookings got canceled.
7. Both hotels have very small percentage that customer will repeat, but Resort hotel has slightly higher repeat % than City Hotel.
8. Travel Agent is most commonly used channel for normal and early bookings.
9. While booking via TA/TO one may have to wait a little longer to confirm booking of rooms.
10. GDS channel brings higher revenue generating deals for City hotel, in contrast to that most bookings come via TA/TO while Resort hotel has more revnue generating deals by direct and TA/TO channel.
11. TA/TO has highest booking cancellation %. Therefore, a booking via TA/TO is 30% likely to get cancelled.
12. Not getting same room do affects the adr, people who didn't got same room have paid a little lower ADR.
13. Avg adr rises from beginning of year upto middle of year and reaches peak at August and then lowers to the end of year.
14. Moslty bookings are done by couples
15. Most people prefer to stay at the hotels of <=7 days.
