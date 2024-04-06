# PrimeNow_DataAnalysis

It dynamically generates column names for the pivot table by concatenating job_number and zip.
It constructs a query to count occurrences of each ASIN and assigns it to the variable @query.
The Counts Common Table Expression (CTE) contains the counts of each ASIN.
The pivot table is generated using the PIVOT function, where the counts are pivoted based on the dynamically generated column names.
The final result of the pivot query is stored in @query.
This code is useful for transforming data from a long format (where each ASIN has multiple rows corresponding to different job_number and zip combinations) to a wide format (where each job_number-zip combination becomes a column, and the counts of each ASIN are populated accordingly).
