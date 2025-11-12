# :e-mail:  Monthly-Email-Marketing-Campaigh 

This project simulates and visualizes the performance of an email marketing campaign using a synthetic dataset generated in Python.
The dataset models customer interactions with marketing emails — including opens, clicks, and purchases — over a two-year period (2023–2024).

The resulting Tableau dashboard presents key engagement metrics by month and a conversion funnel by email type, allowing analysis of campaign performance trends and customer behavior patterns.

## :dart: Project Goals

- Create a realistic synthetic dataset that mimics actual marketing email behavior.
- Explore how open, click, and conversion rates vary by email type.
- Build an interactive Tableau dashboard to visualize campaign performance and trends.

## :dna: Dataset Generation

Using Python and the Faker library, I built a synthetic dataset that simulates customer interactions with marketing emails. Each customer could receive up to 5 emails, one per day, with different message types: 
**Welcome, Promotion, New Product, Cart Reminder, Reactivation**.

For each email, the following events were simulated:
- **Bounce** (2% probability) — message not delivered.
- **Open, Click, Purchase** — with probabilities specific to each email type.
- **Transaction amount** — random value between $500–$1500.

Additionally, I incorporated several mechanisms to introduce realistic variation into the dataset, including:
- **Seasonal effects** — engagement rates were adjusted by month, with higher activity during promotional periods (Jan, Feb, Nov and Dec).
- **Random noise** — added to prevent overly uniform behavioral patterns.
- **Long-term trends** — the overall email open rate increased by around 10% over two years, while the average transaction value grew by about 5%.
- **Purchase behavior** — the average transaction amount varies by email type: Welcome emails tend to generate smaller purchases, whereas Cart Reminder emails lead to higher-value transactions.

## :bar_chart: Tableau Dashboard Features
You can explore the interactive Tableau dashboard [here](https://public.tableau.com/app/profile/alesia.alieva/viz/MonthlyEmailMarketingCampaighConversionRate/DashboardLAST#1).  
In Tableau, a dashboard was built to visualize all **key campaign metrics** on a monthly basis, as well as **the conversion funnel** for each email type.
Additionally, the dashboard includes a **Weekly Conversion Trend**, showing how the conversion rate evolves week by week over the entire campaign period.

<ins>*Interactivity*:</ins>  
*Dropdown* in the top-right corner to select a month.   
*Button* to switch between years.   
*Dynamic filters* automatically update all visuals.  
