# How much money did the most attractive listings generate?
- To find which listings generated the most money, I narrowed down the top 10 listings based on reviews over the last 12 months.
- I looked at data specifically on the most popular property size in each neighborhood.
- Single bedroom listings performed the best in 9 of the top 10 neighborhoods, with Midtown seeing more success with Studio Apartments.
- I created a new column in the Listings sheet called "top_listing" to filter for listings that met this criteria.


###  Next, I calculated how much money the top listings made using the calendar sheet as a way to rank the data.
- First I created a new column in the calendar sheet called "revenue_earned", which represented the revenue earned each night.
- If available was marked as "f" (showing a property was rented), I set "revenue_earned" equal to the "adjusted_price"
- Otherwise the value was set to $0

### Then I took data in the calendar sheet and linked it back to the listings sheet .
- I added a "revenue-earned" column in the Listing sheet, and used the SUMIF() function to copy over the total revenue from the last 30 days.
- To estimate annual revenue, I multiplied the 30-day totals by 12.

### Finally, I built a pivot table that ranked all of the top listings by revenue, using "top_listing" as a filter so I could clearly see which properties were generating the most money.

<img width="714" height="758" alt="image" src="https://github.com/RobertRoddy540/Project-data/blob/main/MHAB&B/Screenshot%202026-06-06%20140805.png?raw=true" />
