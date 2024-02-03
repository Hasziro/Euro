
Euro Exchange Rate Analysis - Code Repository
Overview
This repository contains a Python script for analyzing the Euro exchange rate using historical data. The script performs various data manipulations, calculates moving averages, and exports the data to a MySQL database. Additionally, a simple Tkinter GUI is included to facilitate easy execution of the analysis.

Requirements
Make sure to install the necessary libraries before running the code:

bash
Copy code
pip install numpy pandas requests mysql-connector-python
Script Explanation
1. Downloading and Reading Data
The script starts by downloading historical Euro exchange rate data from stooq.pl. The data is saved as a CSV file and then read into a Pandas DataFrame.

2. Data Manipulations
The script performs various data manipulations, including:

Adding columns for day of the week, abbreviated day, month, and abbreviated month.
Sorting the DataFrame by date in descending order.
Calculating the mean of opening, highest, lowest, and closing rates to create a 'mean' column.
Calculating 30-day, 60-day, and 90-day moving averages.
Determining the maximum closing value in the last 6 months.
3. Descriptive Statistics
The script provides descriptive statistics for the DataFrame, including mean, standard deviation, minimum, and maximum values.

4. Data Export
The DataFrame is exported to a text file named 'file_import.txt'.

5. MySQL Database Connection
The script connects to a MySQL database and inserts the data into the 'euro_kurs' table. Make sure to replace the database connection details and table name with your own.

6. adding moving avg plot 




