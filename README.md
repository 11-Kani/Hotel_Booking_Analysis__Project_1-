# Hotel_Booking_Analysis__Project_1-
Abstract:-
Analyzing the data sheet of hotel bookings and make useful conclusions about general trends in hotel bookings and how factors  like [booking,cancellation,Average daily rate,stay length any many more] governing hotel bookings interact with each other.

Data Summary:-
 Hotel--Contain data values  hotel City ,Resort
is_canceled--Contains  boolean data values 0-->not_canceled 1-->canceled
lead_time--Number of days between the entering date of booking and arrival date
arrival_date_year--Year of the arrival  date of guests
arrival_date_month--Month of the arrival date of guests
arrival_date_week_number--Week number of year of arrival date
arrival_date_day_of_month--Day of the arrival of guests 
distribution_channel--Bookings  done through which distribution channel 
is_repeated_guest--Having values 1🡪repeated guests 0->no repeated guests
previous_cancellations--Number of previous bookings that were cancelled by the guests prior to the current booking
Previous_booking_not_cancellations--Number of previous bookings that were  not cancelled by the guests prior to the current booking
reserved_room_type-- Code for  Room type  values ranges from [A-K] 
Number of changes made to the booking from the moment the booking was entered on the pms(property management system) until the moment of check-in or cancellation
deposit_type--Categorical values—No deposit , Refund, Non-refund
agent--ID of the travel agency made the booking
 Stays_in_weekend_nights--Number of days for stay on weekend night
Stays_in_week_nights--Number of  days for stay on week day 
adults--Number of adults
children--Number of children
babies--Number of babies
meal--Type of meal offered
country--Countries from where guests arrived
market_segment--Categorical values like  TA🡪Travel agent  TO-> Tour Operators
days_in_waiting_list--Number of days the booking was in the waiting list before it was confirmed
customer_type--Categorical values🡪 contract group, transient, party
Average_daily_rate--Obtained by dividing the sum of all lodging transaction by the total number of staying nights
required_car_parking_spaces--Number of car parking spaces used by guests
total_of_special_requests--Number of special requests  made by guests(eg-extra bedsheet)
reservation_status--Contains the current status
total_members--Number of adults + Number of children + Number of babies
Full_stay--Number of stays_in_weekend_nights + Number of stays_in_week_night

Procedure:-
Here in we are dealing with Hotel_Booking_Analysis on to which factors booking,cancellation,profits are decided.
When we  briefly analyze the data sheet we observe some columns with  null values which are  taken care of.We also remove duplicate rows,then we move next target hat is outliers [the exceptional value for particular column which are not relevant for data sheet].Now that our data sheet is void of null values, outliers we can proceed with analysis.
We observe sheet contains data for two types of hotelsCity Hotel & Resort Hotel.We would create a dataframe  subset of each hotel so that we can analyze there inputs separately.

Our observations:
1.For Hotel :-
City Hotel shares 61% out of 100 than Resort Hotel.BB stands for Bed and Breakfast. And 78% of people prefer 'BB' type meal. 'A' is the most preferred room type reserved by guests. . Most of guests visting fall under  Transient Type[it can be individual or group who make booking prior 1-2 days of arrival and their stay length vary from 1-2 days]. Only 8% guests require parking spaces.

2.Bookings and Cancellation:-
Bookings for City hotels are higher than Resort hotels over the years and in year 2016 the bookings for both the hotels were maximum. Most bookings were done in the month of May- August. Most guests visited the hotels where from Portugal and other Europian contries.So we need to advertize more in order countries to gather guests from all over the globe. Only 4% of guests are repeated. This shows industry should encourage honest feedback provided by guest and should create changes  the packages plans and should improvise their  services.Mainly a pair of adults vists the hotel mostly than the family with children. So we can think more of attractive packages for family of 4-5 in offer to increase their engagements. City hotels have more number of stays irrespective of week or weekend stays.

We observed rate of cancellation is higher in City hotel.In year 2015 rate of cancellation was  low. As expected , Most Bookings are done with 'No deposit' and most cancellations are also in 'no deposit' bookings. It is a surprise to see cancellations with 'Non-refundable' bookings. City hotel has significantly longer waiting time, hence City Hotel is much busier than Resort Hotel.

3.Average_daily_Rate:-
We observed: For resort hotels, the average daily rate is more expensive during August- September.For city hotels, the average daily rate is more expensive from May-August .Prices of resort hotel are much higher. Prices of city hotel do not fluctuate that much.

4.Observatin from corelation:
1-->Full_stay length and lead time have slight correlation. This may means that for longer hotel stays people generally plan little before the the actual arrival.2--> Average_daily_rate is slightly correlated with Total_members, which makes sense as more no. of people means more revenue, therefore more Average_daily_rate.
