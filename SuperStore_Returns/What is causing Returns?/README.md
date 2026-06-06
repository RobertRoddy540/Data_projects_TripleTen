## 📋In this section, I built worksheets to analyze different views on return rates.

- I made sure the Returns table was LEFT JOIN’ed onto the Orders table, so I could see both “Yes” and “null” values in the Returned column.💡
- I created a calculated field where the null values became 0 and the Yes values became 1.
- The average of this field represents the return rate, while the total returns equal the count or sum of returns.

🔍 Next, I explored root causes for returned orders by building these worksheets:

- 📈 A scatterplot showing the correlation between total sales and total returns, aggregated by product subcategory. I checked if sales always correlate positively with returns.
- 📊 A bar chart showing the return rate by product category.
- 👥 The return rate by customer, filtering out customers with only 1 order to find those more prone to returns.
- 🗺️ A map showing the return rate by geographic area (state, city, etc.) to identify any location-based concentrations.
- 📅 The return rate by time period (month, week, etc.) to observe any seasonal return trends.
- 🔄 Two composite charts showing return rates across a mixture of factors (date, geography, product category, etc.).

👇Below is the composite chart I made where I combined the Sub-Category, Month, and average rate of returns: 
<img width="402" height="379" alt="image" src="https://github.com/RobertRoddy540/Project-data/blob/main/Screenshot%202026-06-06%20170025.png?raw=true" />
