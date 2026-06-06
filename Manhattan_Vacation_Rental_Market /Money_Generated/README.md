# I wanted to figure out how much money the most attractive listings generated. 
- To do this, I narrowed down my listings to the top 10 neighborhoods based on reviews from the past 12 months. 
- For each of those neighborhoods, I focused on the most popular property size. 
- That worked out to 1-bedroom listings in every neighborhood except Midtown, where studios were the most popular. 
- I added a new column in the listings data called *top_listing*, assigning it a value of 1 if a listing matched those criteria and 0 otherwise.  

### Next, I calculated how much revenue the top listings made using the calendar sheet as the basis for ranking. 
- I started by creating a new column in the calendar data called *revenue_earned*, which records nightly revenue.
- If *available* was marked as "f" (showing a property was rented), I set *revenue_earned* equal to the *adjusted_price*.
- If it wasn’t rented, I made the value $0.  

### After that, I linked the 30-day calendar data back to the listings file. 
- I added a *revenue_earned* column there as well, using a SUMIF() function to bring over the total revenue from the last 30 days.
- To estimate annual revenue, I multiplied the 30-day totals by 12.  

### Finally, I built a pivot table that ranked all of the top listings by revenue, using *top_listing* as a filter so I could clearly see which properties were generating the most money.

<img width="714" height="758" alt="image" src="https://github.com/RobertRoddy540/Project-data/blob/main/MHAB&B/Screenshot%202026-06-06%20123935.png?raw=true" />
