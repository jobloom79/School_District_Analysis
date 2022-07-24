# School_District_Analysis
## School analysis using Anaconda and Jupiter
### Overview of Project:
---The School Booard has found evidence of grade tampering and as a result the Schoole District Analsys is being redone with the compromised grades srubbed
### Analysis and Challenges:
#### Deliverable 1: Replacing Thomas High School Ninth-Greade Math and Reading Scores
---This challenge was relatively simple using the 'loc' method with 'conditional statements' to find and replace Thomas High School grades wtih NaN valus using 'np.nan' value.
Once replaced a new school_data_complete_df dataframe was created using 'pd.merge' function in the Pandas dependency to merge the student data to the school data on the "school_name" column.
#### Deliverable 2: Repeat the School District Analysis
---This deliverable proved to be the most challenging due figuring out how to get the new table calculated with the missing data. Several errors were discovered attmepting to using the loc method with replace and other attempts based on research on replacing data. The attempt was to replace an entire row of student values for Thomas High School in the "per_school_summary" dataframe as opposed to replacing the specific values within that Thomas row. Once the specific values wer replaced the new school_summary was able to be used to further calculate scores by grade,spending, school size and type.
### Results: 
---The first results noticed is the District Summary showed a slught drop in rating across the board with Passsing Percentage for Math having the most detriment at two-tenths of a percentage point decrease. 

![District Summary](https://github.com/jobloom79/School_District_Analysis/blob/main/Resources/district_summary.png)

---The school summary's affects were nominal with the math scores, but the most interesting discovery was the "Average Reading Scores" for Thomas High School increased while the "Passing percentage" for reading decreased.

![School Summary](https://github.com/jobloom79/School_District_Analysis/blob/main/Resources/school_summary.png)

--The same results can be found in reviewing the scores by School Spending,School size and School Type. The changes of each category is nominal leaving each category relatively unchanged
![School Spending](https://github.com/jobloom79/School_District_Analysis/blob/main/Resources/spending_summary.png)

![School Size](https://github.com/jobloom79/School_District_Analysis/blob/main/Resources/school_size.png)

![School Type](https://github.com/jobloom79/School_District_Analysis/blob/main/Resources/school_type.png)
### Summary: 
---After reviewing the data we have come to the conclusing that there is little to no evidence of academic dihonesty as the grades were mostly unaffected and in the category of average reading scores increasing while the percent passing decreased, shows there was a large enough number of grades that were borderline passing for Thomas High School 9th grade to bring down the School average if they were included. 
