This project analyzes a café dataset sourced from Kaggle. The primary goal is to clean, process, and visualize the data to extract actionable insights using Python libraries such as Pandas and Matplotlib.

This project involves:

Data Cleaning: Handling duplicates, null values, and erroneous entries.
Data Analysis: Grouping data to understand key metrics such as top-selling items, payment methods, and transaction trends.
Data Visualization: Using Matplotlib to create bar charts, line plots, and pie charts that provide a clear visual summary of the café's operations.
Dataset

The dataset used in this project (dirty_cafe.csv) is a collection of transactional data from a café. Key fields include:

Transaction ID
Item
Quantity
Price Per Unit
Total Spent
Payment Method
Location
Transaction Date
Installation

Make sure you have Python installed. It’s recommended to create a virtual environment. Install the required libraries using pip:

pip install pandas matplotlib
Project Structure

├── dirty_cafe.csv     # The dataset file
├── analysis.py        # The Python script for data cleaning, analysis, and visualization
└── README.md          # This file
Data Cleaning

Key steps in cleaning the data:

Duplicate Check: Identify and remove duplicate entries based on Transaction ID.
Handling Null Values: Use forward fill (ffill) and backward fill (bfill) to handle missing values.
Data Replacement:
Replace "UNKNOWN" with "Pizza" (for Item) and with "Cash" (for Payment Method).
Replace "ERROR" with appropriate values (e.g., "Pasta" for Item, numeric defaults for Quantity, Price Per Unit, and Total Spent).
Type Conversion: Convert Total Spent to numeric and Transaction Date to a datetime object.
Analysis & Visualizations

Item Analysis
Grouping: Data is grouped by Item to compute the sum of Total Spent and count of Quantity.
Visualization: A bar chart is created to display total sales and the number of transactions per item.
Monthly Sales Trend
Date Extraction: The month is extracted from the Transaction Date for grouping.
Visualization: A line plot with markers visualizes total sales trends over time.
Payment Method Analysis
Grouping: Data is grouped by Payment Method to count the number of transactions.
Visualization: A pie chart is generated to show the distribution of payment methods.
Location Analysis
Grouping: Data is grouped by Location (e.g., dine-in vs. takeaway) to compare transaction counts and total sales.
Visualization: A bar chart displays insights on where customers prefer to dine.
Usage

To run the project, execute the following command in your terminal:

python analysis.py
This script will:

Read and clean the dataset.
Generate various visualizations for data insights.
Display the charts using Matplotlib.
Results

The analysis revealed:
Top-selling Items: Identifying which menu items contribute the most to total sales.
Payment Preferences: Visual insights into the most commonly used payment methods.
Monthly Sales Trends: Understanding how sales fluctuate over time.
Dine-in vs. Takeaway: Insights into customer preferences regarding the mode of service.
Contributing:
Contributions, suggestions, and improvements are welcome! Please open an issue or submit a pull request.

Contact
For questions or further discussion, please reach out at:
Email: basu6607@gmail.com
LinkedIn: https://www.linkedin.com/in/basu-sharma-543392186/
