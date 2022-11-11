

# 370 Final Project
Project progess and notes denoted below.

~~Strikethrough completed tasks.~~

# TO-DO

## ~~Question 1 - Download Data~~ 
~~1. Download data from NBER site~~ 

~~2. Create hcris_raw directory for final project~~

~~3. Implement "Switch" in code that indicates whether or not data should be downloaded (prevent multiple downloads with multiple runs)~~

## Question 2 - Cleaning the Data
Overview: extract variables, merge data, clean data
### Reformatting The Raw Data
~~Read in CSVs~~
1. Create key for variables (to merge) 
2. Convert long to wide data 
3. Merge two variables from rpt data 
4. Add "year" as a variable 
5. Save resulting data as a hcris.YEAR.csv
6. Check: Two subdirectories in main directory, 13 files in cleaned folder 

### Clean The Reformatted Data 
Options:  
1. Read in 1998 data as hcris_data. Loop and rbind
2. list.files(), lapply(), fread()

Then: 
1. Drop observations without prvdr_num 
2. Replace negative costs with absolute 
3. Replace missing values with 0 for epo_rebates 
4. Make sure epo_cost is a numeric variable 
5. Make sure epo_cost > epo_net_cost for all observations (swap)
6. Change observations where prvdr_num == 322664 to 342664 
7. Clean dates 
8. Drop report_start_date, report _end_date and replace with fy variables 
9. Clean zip codes 
10. Clean missing states 
11. Create chain_id indicator variable 
12. Remake chain_indicator with cleaned variale chain_identity 

## Question 3 - Analysis 
1. Analyze how chains differ from independent clinics in their costs/behavior (at least ~half a page of writing)

## Notes for presentation: 
NULL
