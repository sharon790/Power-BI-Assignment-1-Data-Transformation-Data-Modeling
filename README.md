# Power-BI-Assignment-1-Data-Transformation-Data-Modeling
I transformed the "LIST_OF_ORDERS" to power query and restricted the data till 500 rows by using   { >home>keep rows>tops rows>500. }
I changed the data type of 'Order_Date' to "DATE". and "Amount" & "Target" to 'Fixed decimal Number
Formatted the 'Customer_name' to capitalizing each word by using {  >Transform>Format>capitalize each word  }
Selected the columns both " city" & "State" into one with one delimitor 'comma'
I added a column {  >add column >custom column >profit/amount  } then changed the Data type to ' Percentage'
I created a new custom column named it as ' Profit_ Status' {  if [profit] <0 then "Loss" else if [profit] =0 then " Break-Even" else " Profit"  }
I merged the two tables using {  >Home >Merge queries as new > selected the other table (order details) > selected the common column > unticked the common column (Order_ID) > unticked 'Orginal column name as prefix'.
when i checked i could not find any missing values and for duplicate rows i selected the entire table and > remove rows > remove duplicate values
To sort , i clicked the drop down of Order Date and pressed the descending
Filtered the "Location " by using text filter >contains >'Tamil Nadu'
I Duplicated the table ' Order details' and calculated the count of each 'Order_ID' using   >transform >Statistics >count distinct values = 500
After finding average profit by each Category  by sung group function : furniture -9.456790123 , cloths -11.76290832, Electronics -34.07142857
Month of Order Date  -	total target by month
01-04-2018	31400
01-05-2018	31500
01-06-2018	31600
01-07-2018	33800
01-08-2018	33900
01-09-2018	34000
01-10-2018	36100
01-11-2018	36300
01-12-2018	36400
01-01-2019	43500
01-02-2019	43600
01-03-2019	43800
