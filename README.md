# VLOOKUP-XLOOKUP-PIVOT-Practice-Questions
# Project Overview
## I have practiced basic VLOOKUP, XLOOKUP, and PIVOT Functions by using these functions to:
- Match employees with their departments (Locating employee directory)
- Match individual employees with their sales amount (KPI)
- Match sales to their specific area (Regional sales analysis)
- Calculate average sales for each location, with function to filter by region 

# Sample data
| Employee ID | Name    |  Department  |  Location  |  Sales ($)  |
|-------------|---------|--------------|------------|-------------|
|   101       | Alice   |  HR          |  London    |  5000       |
|   102       | Bob     |  Finance     |  Boston    |  7000       |
|   103       | Charlie |  IT          |  Seattle   |  6000       |
|   104       | Diana   |  Marketing   |  Chicago   |  8000       |
|   105       | Ethan   |  Sales       |  Boston    |  9000       |


# Scenarios and Answers
## Q1: What is the department of employee ID 103?			
- Formula:	 VLOOKUP(A8,A6:E10,3,FALSE)		
- Answer:	IT		
			
## Q2: How much did Diana made in sales?			
- Formula:	VLOOKUP(B9,B6:E10,4,FALSE)		
- Answer:	8000	$	
			
## Q3: Use IFERROR to return "Not Found" if ID 106 is searched.			
- Formula:	IFERROR(VLOOKUP(106,A6:E10,2,FALSE), "Not Found")		
- Answer:	Not Found		
			
			
## Q4: What is the location of Employee ID 105?			
- Formula:	XLOOKUP(105,A6:A10,D6:D10)		
- Answer:	Boston		
			
## Q5:What is the name of the employee who works in marketing?			
- Formula:	XLOOKUP("Marketing",C6:C10,B6:B10)		
- Answer:	Diana		
			
## Q6:Find the department of ID 108, return "Invalid ID" if not found			
- Formula:	XLOOKUP(108,A6:A10,C6:C10,"Invalid ID")		
- Answer:	Invalid ID		
			
## Q7:What is the total sales for each department?			
- Answer: Refer to PIVOT Table in data uploaded

## Q8: What is the  average sales in each location?
- Answer: Refer to PIVOT Table in data uploaded

## Q9:What is the average sales for Boston area only?
- Answer: Refer to PIVOT Table in data uploaded

# Conclusion
- VLOOKUP: Can be used for simple and fast lookups. Suitable for sharing with older Excel versions.
- XLOOKUP: Can be used for flexible lookups, has built-in error handling. It is more modern and more comprehensive than VLOOKUP. Might not be compatible with older Excel versions.
- PIVOT Tables: Can be used to summarise, group and analyse large datasets
