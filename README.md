# Project Summary
The aim of this project was to perform exploratory data analysis (EDA) on a hotel booking dataset in order to gain insights into customer behavior and booking patterns. The dataset consist of 119390 rows and 32 columns in which it contained information on hotel bookings, cutomer types, distribution channel, customers types ,country, meal and many more. First we imported all the essential pyhton libraries and load the 'Hotel_Booking_Data' dataset then we cleaned our data by removing duplicate values, visualizing missing value and fill null values then we added few columns for our visualization and finally we visualized the data by using various graphical techniques such as bar plot, count plot, pie chart and heat map. Through our analysis, we discovered several interesting insights. For example, that our revenue is getting decreased after year 2016.
# Problem Statement
* What is the Revenue per year for Each Hotel?

* What is the Booking percentage of each type of hotel?

* What is Average Days stay by customer in both type of Hotels?

* What is the most popular Market Segment in both Hotels?

* What is the Revenue by each distribution channel?

* What is the Most popular meal type percentage?

* What is the Average Monthly Rate?

* How many time a room has been assigned?

* What is the monthly Cancellation count for both Hotels?

* Which top 15 countries generate highest revenue?

* Which Agent has most no of bookings?

* What is Repeated Guest Percentage?
# Library 
###  `Pandas`
###  `Numpy`
###  `Matplotlib`
###  `Seaborn`
###  `Datetime`
###  `Calendar`
# My Dataset tells me about 
This data set contains a single file which compares various booking information between two hotels: a city hotel and a resort hotel.Includes information such as when the booking was made, length of stay, the number of adults, children, and/or babies, and the number of available parking spaces, among other things. The dataset contains a total of 119390 rows and 32 columns.Dataset Contains duplicated items i.e 31944 which is removed later .In this dataset we find data types of every columns i.e (Int, float ,string) and observe that some columns data types is not accurate and remove later .We find unique value of every columns it means what actual values in every columns
# Variables Description
The columns and the data it represents are listed below:

hotel : Name of the hotel (Resort Hotel or City Hotel)

is_canceled : If the booking was canceled (1) or not (0)

lead_time: Number of days before the actual arrival of the guests

arrival_date_year : Year of arrival date

arrival_date_month : Month of month arrival date

arrival_date_week_number : Week number of year for arrival date

arrival_date_day_of_month : Day of arrival date

stays_in_weekend_nights : Number of weekend nights (Saturday or Sunday) spent at the hotel by the guests.

stays_in_week_nights : Number of weeknights (Monday to Friday) spent at the hotel by the guests.

adults : Number of adults among guests

children : Number of children among guests

babies : Number of babies among guests

meal : Type of meal booked

country : Country of guestsAnswer Here

market_segment : Designation of market segment

distribution_channel : Name of booking distribution channel

is_repeated_guest : If the booking was from a repeated guest (1) or not (0)

previous_cancellations : Number of previous bookings that were cancelled by the customer prior to the current booking

previous_bookings_not_canceled : Number of previous bookings not cancelled by the customer prior to the current booking

reserved_room_type : Code of room type reserved

assigned_room_type : Code of room type assigned

booking_changes : Number of changes/amendments made to the booking

deposit_type : Type of the deposit made by the guest

agent : ID of travel agent who made the booking

company : ID of the company that made the booking

days_in_waiting_list : Number of days the booking was in the waiting list

customer_type : Type of customer, assuming one of four categories

adr : Average Daily Rate, as defined by dividing the sum of all lodging transactions by the total number of staying nights

required_car_parking_spaces : Number of car parking spaces required by the customer

total_of_special_requests : Number of special requests made by the customer

reservation_status : Reservation status (Canceled, Check-Out or No-Show)

reservation_status_date : Date at which the last reservation status was updated

total_night_stay : Number of total nights (week night+ weekend night) spent at the hotel by the guests.

revenue: Revenue genrated by the customer calculated by adr * total_night_spent.

total_guest : Total no of Guest stayed in the hotel
# Data Pre-Processing steps performed
We deleted duplicated values from our Dataset

we filled all null value columns with some values

We wanted to changed the data type of column agent and children from float to Int and we changed the data type of reservation_status_date colomn from object to datetime

we have replaced 0 and 1 with 'not canceled' and 'canceled' and 'Not a repeated guest' and 'repeated guest' in coloumn 'is_canceled' and 'is_repeated' respectively

We added 5 new columns listed below

Total_night_stay that is Total_week_night + total_weekend_night
Revenue that is Adr * Total_night_stay
Total_guest that is adults + children + babies
We have converted Year coloumn into datetime formate and extract year and month out of it
# Solution to Business Objective
What do you suggest the client to achieve Business Objective ?
Explain Briefly.

Based on our business goals and the problems we aimed to address, we used bar plots, count plots, pie charts, and heat maps to visualize the issues. We discovered important insights, which are explained with their respective charts above. Additionally, we have suggested some solutions to better understand our customers and improve our services efficiently.
# Conclusion
Based on the problem statements mentioned above, we have analyzed the following insights:

The revenue trend increased until 2016 for both types of hotels and then experienced a downward trend.

Overall, the City Hotel accounts for 61% of bookings, while the Resort Hotel makes up 38% of bookings.

Contract-type customers have the longest average stay at the resort hotel, which is 8 days.

The maximum number of bookings comes from the online Travel Agency (TA) medium, totaling 34,994.

We receive most of the revenue from the TA/TO distribution channel in both hotels.

Bed and Breakfast is the most popular meal type, comprising 78% of bookings.

November and December have the lowest Average Monthly Revenue (AMR), with figures of 76.75 and 77.06, respectively, while August boasts the highest AMR at 145.49.

Room type 'A' has the highest assigned count, with 16,313 bookings.

March has the highest number of booking cancellations, totaling 2,652.

Portugal generates the highest profit in revenue for us.

Agent with ID number 9 brings in the highest number of bookings, which is 28,759.

We have only 4% of repeat guests, and there is a need to improve our facilities in both hotels to increase the percentage of repeat guests.
