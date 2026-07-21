# Magical Chocolate Co.

This project uses business data from a generator for the fictional company Magical Chocolate Co.: https://excelx.com/practice-data/generators/business-data/

The generator gives various options for choosing clean vs messy data and some data has the option of being random or having built in trends. As a cleaning exercise, I downloaded the Detailed Expense Ledger with 2000 rows and 15% errors. First I cleaned the data in Excel and then I replicated the cleaning in SQL. My cleaning methodology is described in the Excel file and the SQL query file is attached separately. The two results are not exact matches but they're reasonably close. The Excel cleaned data has 1610 rows while the SQL cleaned data has 1614 rows. It was more difficult in SQL than Excel to tackle the challenge of choosing which duplicate to preserve. Given the nature of the data and the relatively small dataset, I would choose the manual Excel cleaning in the future. 

