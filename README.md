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

![Email Campaign Dashboard](https://private-user-images.githubusercontent.com/77228507/513427712-1a91ba0d-85a3-49c8-bbbe-96a44e31efb5.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NjI5NjU1NDUsIm5iZiI6MTc2Mjk2NTI0NSwicGF0aCI6Ii83NzIyODUwNy81MTM0Mjc3MTItMWE5MWJhMGQtODVhMy00OWM4LWJiYmUtOTZhNDRlMzFlZmI1LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTExMTIlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUxMTEyVDE2MzQwNVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWM0NWFlOWU1N2E1ODQ1M2NkZTg2MTM1ZWVkNWM2NDBmY2MxYTNmNDBmYmM1ZjRjYzcwYWEwYjkxMDBlMzQ4NzMmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.TSmsA4wpQFGIqQxjOZ5EdwWzFUe4c-Thts-HB6CmjJE)

In Tableau, a dashboard was built to visualize all **key campaign metrics** on a monthly basis, as well as **the conversion funnel** for each email type.
Additionally, the dashboard includes a **Weekly Conversion Trend**, showing how the conversion rate evolves week by week over the entire campaign period.

<ins>*Interactivity*:</ins>  
*Dropdown* in the top-right corner to select a month.   
*Button* to switch between years.   
*Dynamic filters* automatically update all visuals.  
