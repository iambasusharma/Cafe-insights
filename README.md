Overview

This project involves cleaning a dataset by handling missing and erroneous values and then visualizing key insights using Matplotlib. The dataset includes information about transactions, including items purchased, quantities, prices, payment methods, and transaction dates.

Features

Data Cleaning

Replaced missing or erroneous values in columns like Item, Quantity, Price Per Unit, Total Spent, Payment Method, and Location.

Used forward fill (ffill) and backward fill (bfill) techniques to handle missing values.

Converted Transaction Date to a datetime format, handling errors appropriately.

Data Aggregation

Grouped data by Item to calculate total spending and quantities sold.

Grouped data by Month to calculate total sales per month.

Grouped data by Payment Method to analyze the frequency of different payment options.

Data Visualization

Bar Chart: Total sales for each item, with item names and quantities labeled.

Line Chart: Monthly sales trends over a year.

Pie Chart (not shown in the code, but can be implemented): Payment method distribution.
