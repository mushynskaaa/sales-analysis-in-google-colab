# Sales Analysis by Product, Geography, and Time
A deep dive into the company's sales and revenue, based on order data from multiple countries (2010–2017). The analyst's full workflow, from data cleaning to visualizations and recommendations.

## Project Objective
Analyze sales from several different perspectives: product categories, countries, subregions, sales channels, and time. Identify trends and formulate recommendations for the business.

## Data
Three related tables combined into a single DataFrame:
- **events** - information about the orders themselves (date, country, product, quantity, price, cost, channel)
- **products** - information about product categories
- **countries** - information about countries, including their codes and sub-regions

## Stack
Python (pandas, numpy), matplotlib, seaborn. Environment: Google Colab.

## Tasks Completed in This Project

**Data Cleaning**
- Handling missing values (median / “Unknown” / removal based on key)
- Type conversion (dates from Object to datetime)
- Checking for explicit and implicit duplicates (case sensitivity, spaces)
- Explicit anomaly checks (shipment dates, price and cost of goods sold (does the latter exceed the former?), zero sales)
- All actions performed while ensuring the preservation of the Namibia (NA) country code and handling invalid country codes

**Analysis and Visualization**
- Key metrics: revenue, cost of goods sold, profit, margin
- Sales by category, country, subregion, and channel
- Delivery time and its correlation with profit
- Sales trends over time (by year, with data completeness checks)
- Analysis by day of the week and seasonality

## Key Findings

- Revenue leaders are not always profit leaders; high cost of goods sold results in lower margins (e.g., Czech Republic)
- Some countries are unstable (due to dependence on one-time large orders), while subregions are stable due to averaging
- Delivery time does not correlate with profit
- No products with pronounced seasonality were identified, and sales are evenly distributed across the days of the week
- Data for 2017 is incomplete (through July 23); this has been factored into all forecasts and conclusions

## Get in touch
Feel free to connect on [LinkedIn](https://www.linkedin.com/in/yuliia-mushynska-a31141346), or check out more dashboards on [Tableau Public](https://public.tableau.com/app/profile/yuliia.mushynska).
