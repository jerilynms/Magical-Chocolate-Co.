# Magical Chocolate Co.

This project uses business data from a generator for the fictional company Magical Chocolate Co.: https://excelx.com/practice-data/generators/business-data/

The generator gives various options for choosing clean vs messy data and some data has the option of being random or having built in trends. With the exception of the data cleaning exercise, I downloaded clean data with 2000 rows and dated between 1/1/2022 and 7/17/2026. 

### Data Cleaning
As a cleaning exercise, I downloaded the Detailed Expense Ledger with 2000 rows and 15% errors. First I cleaned the data in Excel and then I replicated the cleaning in SQL. My cleaning methodology is described in the Excel file and the SQL query file is attached separately. The two results are not exact matches but they're reasonably close. The Excel cleaned data has 1610 rows while the SQL cleaned data has 1614 rows. It was more difficult in SQL than Excel to tackle the challenge of choosing which duplicate to preserve; however, with a larger dataset, the SQL queries would be the most efficient. 

### Finance & Accounting Dashboard
This dashboard has three pages based on the Detailed Expense Ledger and Accounts Receivable Aging Report. The summary page calls out the company's total revenue, expenses, and profit/losses, which can be filtered by year. The column chart visualizes those figures for the last five years. 2023 had the highest revenue and profit year. There is also a pie chart the visualizes how much revenue is sitting in unpaid customer invoices. There are navigation buttons to take you to the other two pages of the dashboard. 

**<ins>Methodology:</ins>** I created a column in both tables to isolate the year of the invoice and expenditures so that I could link the tables based on time and would be able to filter the data based on year. In the Accounts Receivable table I created a revenue column based that assigned $0 to unpaid invoices. I also created a column based on if the invoice was unpaid and past it's due date with either Yes, No, or Null. I also calculated a column for the number of days the invoice was past due. I then created a new table based on the overdue invoices column so that I could isolate the data for all overdue invoices, which informs the third page of the dashboard. I also created several measures which can all be found in the callout cards on each of the dashboard pages.  

