
# Applied Data Analytics

## Wedge Project

Finally, a first draft of the Wedge. Many apologies for my tardiness. You were right that this was a project worth starting 6 weeks ago.

### Task 1

* Files for this task: 
`Wedge_File_Cleaning.ipynb`: 
This is the central file for all of the cleaning. It takes the files from the ZipFiles folder and brings all of them to a new folder `CleanFiles`, at which point they can be uploaded to GBQ


### Task 2

* Files for this task: 

`Wedge_Owner_Sample.ipynb`:
This file runs a query in GBQ to extract a sample of 200 owners, and writes this sample to a local textfile
	

### Task 3

* Files for this task: 

`Summary Tables.ipynb`:
This file writes each query in GBQ, writes the results to a local textfile, creates a SQL database, and imports each textfile as a table in that database


`Wedge_Sum_Files.db`:
This is the database for the summary tables


## Query Comparison Results

Fill in the following table with the results from the 
queries contained in `gbq_assessment_query.sql`. You only
need to fill in relative difference on the rows where it applies. 
When calculating relative difference, use the formula 
` (your_results - my_results)/my_results)`. 



|  Query  |  Your Results  |  My Results | Difference | Rel. Diff | 
|---|---|---|---|---|
| Total Rows  |  85760124 | 85760139   |  15 | 0  |
| January 2012 Rows  |  1070907 |  1070907 |  0 |  0 |
| October 2012 Rows  |  1042287 | 1042287  |  0  | 0 |
| Month with Fewest  |  February | February  | Yes  | NA  |
| Num Rows in Month with Fewest  | 6556769  | 6556770  | 1  | 0  |
| Month with Most  | May  | May  | No  | NA  |
| Num Rows in Month with Most  | 7578371  |  7578372 |  1 |  0 |
| Null_TS  | 7123776  |  7123776 | 0  |  0 |
| Null_DT  |  0 | 0 | 0  |  0 |
| Null_Local  |  234839 |  234839 | 0  | 0  |
| Null_CN  | 0  |  0 |  0 |  0 |
| Num 5 on High Volume Cards  | 14987.0  | 14987.0  | Yes  | NA  |
|  Num Rows for Number 5 |  460625 |  460630 | 5  |  0 |
| Num Rows for 18736  | 12153  |  12153 | 0  | 0  |
| Product with Most Rows  | banana organic  | banana organic  | Yes  | NA  |
| Num Rows for that Product  |  908637 |  908639 | 2  | 0  |
| Product with Fourth-Most Rows  |  avocado hass organic |  avocado hass organic | Yes  | NA  |
| Num Rows for that Product  | 456771  |  456771 | 0  |  0 |
| Num Single Record Products  |  2741 | 2769  |  28 |  .01 |
| Year with Highest Portion of Owner Rows  |  2010 |  2010 | Yes | NA |
| Fraction of Rows from Owners in that Year  |  0.7422 |  0.7422 |  0 |  0 |
| Year with Lowest Portion of Owner Rows  | 2017  |  2017 | Yes  | NA |
| Fraction of Rows from Owners in that Year  |  0.7513 | 0.7513  |  0 |  0 |

## Reflections

This project was exhausting but ultimately extremely rewarding. I had to work through the file cleaning multiple times, which took probably 20 hours of work, and I still have a couple rows off, as shown on the queries I ran below. Overall, it is much closer than my first attempt, which saw me off by millions of rows and unable to complete the summary tables. I chose to use pandas for the project, and I'd love to talk about how else I might have gone about cleaning the files. 

I think there are some issues with my summary tables. I'd love to go over the queries with you in an office hours session if you have the time.
