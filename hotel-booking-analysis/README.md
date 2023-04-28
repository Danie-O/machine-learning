## Exploratory Data Analysis of the Hotel Booking Dataset

About the Dataset
-----------------
Number of features: 32
Number of observations: 119390
Features: ['hotel', 'is_canceled', 'lead_time', 'arrival_date_year', 'arrival_date_month', 'arrival_date_week_number', 'arrival_date_day_of_month', 'stays_in_weekend_nights', 'stays_in_week_nights', 'adults', 'children', 'babies', 'meal', 'country', 'market_segment', 'distribution_channel', 'is_repeated_guest', 'previous_cancellations', 'previous_bookings_not_canceled', 'reserved_room_type', 'assigned_room_type', 'booking_changes', 'deposit_type', 'agent', 'company', 'days_in_waiting_list', 'customer_type', 'adr', 'required_car_parking_spaces', 'total_of_special_requests', 'reservation_status', 'reservation_status_date']

Data Preparation and Cleaning
----------------------------
- Loaded the dataset into a DataFrame and made a copy of the original dataset.
- Explored the size of the dataset and checked for the statistical summary.
- Checked for missing values in each column and calculated the percentage of missing values.
- Replaced null values in the 'children' column with 0, as it is likely that no children stayed the night.
- Replaced null values in the 'country' column with the most common value (mode).
- Replaced null values in the 'agent' column with 0, as NaN in the 'agent' column indicates that the booking was made without an agent.
- Dropped the 'company' column due to a high percentage of missing values.
- Dropped rows where the sum of 'adults', 'babies', and 'children' columns is 0, as these bookings had no actual guests.
- Converted the 'children' and 'agent' columns to integer data type.

Data Exploration
----------------
- Analyzed the cancellation rate for bookings by hotel type.
- Plotted the number of bookings by year and hotel type.
- Calculated and plotted the cancellation rate by hotel type.
- Explored the distribution of customer types and plotted it.
- Explored the customer type distribution by hotel type.
- Explored the relationship between market segment and length of stay on weekdays.
- Plotted the average daily rate (ADR) by market segment.
- Analyzed the distribution of lead time (number of days between booking and arrival) and plotted it.
- Explored the distribution of total number of special requests and plotted it.
- Explored the relationship between total number of special requests and hotel type.
- Analyzed the average number of bookings per month and plotted it.
- Analyzed the average daily rate (ADR) and plotted it.
- Explored the relationship between lead time and cancellation rate.
- Explored the relationship between deposit type and cancellation rate.
- Explored the relationship between customer type and cancellation rate.
- Explored the relationship between market segment and cancellation rate.
- Explored the relationship between distribution channel and cancellation rate.
- Explored the relationship between reserved room type and cancellation rate.
- Explored the relationship between assigned room type and cancellation rate.
- Explored the relationship between booking changes and cancellation rate.
- Explored the relationship between required car parking spaces and cancellation rate.

### *Results of analysis are embedded in the notebook*
