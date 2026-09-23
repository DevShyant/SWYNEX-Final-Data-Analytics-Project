# SWYNEX-Final-Data-Analytics-Project
Problem Statement

Retail and e-commerce brands operating across multiple online marketplaces (Amazon, Flipkart, Myntra, Meesho, Ajio, Shein) and offline channels struggle to get a unified view of who is buying, what they're buying, where they're buying from, and how delivery, discounts, and payment choices affect purchase behavior.

Data Cleaning Process

Performed in Jupyter Notebook (SWYNEX_EDA.ipynb) using pandas:

Loaded the raw data with pd.read_csv() and inspected structure using df.head(), df.info(), and df.describe().
Checked for missing values (df.isnull().sum()) and handled nulls in fields like Discount, Color, or Delivery Time — either imputed or dropped depending on the column.
Removed duplicate transactions using df.duplicated() / df.drop_duplicates().
Standardized categorical values — trimmed whitespace and fixed inconsistent casing/spelling across Location, Online Store, Brand, and Category (e.g. "flipkart" vs "Flipkart").
Fixed data types — converted Purchase Date to datetime, ensured Age, Quantity, Purchase Amount, and Discount (%) were numeric.

Analysis

Exploratory analysis was carried out in Python (pandas, seaborn) inside SWYNEX_EDA.ipynb, covering:

Univariate analysis: distribution of age, purchase amount, and discount
Channel analysis: online vs offline order counts and revenue split
Category/brand analysis: top-selling categories, items, and brands by revenue and quantity
Geographic analysis: order volume and revenue by city
Demographic analysis: purchase behavior by gender and generation
Delivery analysis: relationship between delivery speed, delivery time, and order value

Dashboard

Built in Power BI (SWYNEX_Dashboard.pbix), with the following views:

Online vs Offline split (donut chart)
Gender split (donut chart)
Payment Method distribution (donut chart)
Sum of Purchase Amount by Online Store (bar chart) — Flipkart, Myntra, Amazon, Meesho, Ajio, Shein, Others
Orders by Location (tree map) — Pune, Chennai, Mumbai, Bangalore, Hyderabad, Kolkata, Delhi, Chandigarh, Ahmedabad, and more
Count of Generation by Generation (donut chart) — Gen-Z vs Other
Count of Delivery Speed by Delivery Speed (bar chart) — Same Day, Express, Standard
Category filter buttons — Accessories, Footwear, Clothing
