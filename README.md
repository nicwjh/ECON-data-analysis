# 370 Final Project
Project progess and notes denoted below.

~~Strikethrough completed tasks.~~

# TO-DO
Next task: 

## ~~Question 1 - Download Data~~ 
~~1. Download data from NBER site~~ 

~~2. Create hcris_raw directory for final project~~

~~3. Implement "Switch" in code that indicates whether or not data should be downloaded (prevent multiple downloads with multiple runs)~~

## Question 2 - Cleaning the Data
Overview: extract variables, merge data, clean data

~~Reformatting The Raw Data~~

~~Read in CSVs~~

~~1. Create key for variables (to merge)~~

~~2. Convert long to wide data~~

~~3. Merge two variables from rpt data~~

~~4. Add "year" as a variable~~

~~5. Save resulting data as a hcris.YEAR.csv~~

~~6. Check: Two subdirectories in main directory, 13 files in cleaned folder~~

### Clean The Reformatted Data 
~~Options:~~
  
~~1. Read in 1998 data as hcris_data. Loop and rbind~~

~~2. list.files(), lapply(), fread()~~

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

**On completion: remember to delete hcris raw

## Notes 11/17 
observation in final data: provider_num, year -> rpt_num 

each provider number & year has a unique rpt_num

rpt_num -> worksheet, line, column, value 

rpt_num -> prvdr_num, year, var1, var2

provider number and year map to report number

report number maps to a worksheet, line, column, value. 

check Alex's chart he uploaded 

nmrc and alpha have values in the data

use worksheet, line, coluimn to map to variable codes that Alex gave to get variable names 

chain_identity: important to know what chains own the clinics

epo variable: be careful. some people don't report it correctly 

one strategy: epo_total * 1000 / cost ~ $8-12. if not in this range, can delete 
- in documentation, don't spend too much time on this 

listen to the podcast(first 25 minutes)/read the paper for context 

Freakonomics podcast: 



strategy: 

## Notes for presentation: 
NULL
