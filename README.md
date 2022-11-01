# School District Analysis

## Overview of the Project

### Purpose  
Maria is the chief data scientist of her city’s school district, and she needs help analyzing data on school funding and standardized test scores. Using the dataset provided, we will be aggregating the data to showcase trends in school performance by completing the following tasks: 

1) Collect and place the student data into a DataFrame. 
2) Prepare and clean the DataFrame. 
3) Summarize key aspects of the data.
4) Analyze specific subsets of data. 
5) Compare and contrast the data. 

## Resources 
- Data Source: new_full_student_data.csv
- Software used: Python 3.9.7, Jupyter Notebook 6.4.12 and Pandas 1.3.5

## Summary of Findings 

During this analysis, I found that the reading and math scores had some null values, and the dataset has a few duplicate rows that needed to be dropped before the analysis could begin. The “grade” variable was misclassified as an object datatype because there were non-numeric variables (the "th" in 9th, 10th, 11th, and 12th) that needed to be removed so the datatype could be changed to an “integer”. 

Using the `describe` function, a summary of the data showed that: 
-	The average reading score amongst all students in the dataset is 72.35.
-	The mean math score of all students in the dataset is 64.67. 
-	The lowest reading score found in the dataset is 10.5.

When taking a closer look at the descriptive statistics with the `loc` and `iloc` functions, the results showed: 
-	The average reading score of all 9th graders is 69.24, and the average math score is 66.58.
-	Matthew Thomas, a 10th grader from Dixion High School has the lowest reading score in the dataset with a 10.5.
-	The mean reading score for all 11th and 12th graders is 74.9.

When comparing District schools and Charter schools primarily using the `groupby` function, the analysis showed that:
-	Public schools had a higher school budget ($911,195) than Charter schools ($872,625).
-	Montgomery High School had the most students (2038) while Chang High School had the least (171).
-	Charter schools had higher math scores (except for 12th grade) than Public Schools.
