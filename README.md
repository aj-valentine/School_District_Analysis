# School District Analysis with Jupyter Notebooks + Pandas

## Overview of the School District Analysis :notebook:
This project was created for Maria, a chief data scientist for a city school district, in hopes of generating analysis about school and district level funding and students' performance in standardized test scores. We were given two sets of data in csv files, one that contained student math and reading scores and their school information, and another that provided detailed information about the 15 schools in study. We aggregated the data into one dataframe in order to show trends in school performance based on their funding levels. Once this data was combined, we had to take out the ninth-grade reading and math scores for Thomas High School because there was an issue with academic dishonesty and someone had altered the test scores. With these removed, we were able to analyze the data without the altered information. In the results, we provide seven different dataframes of information: a district summary across all 15 schools with reading and math performance, a school summary that breaks down the testing performance by high school, the top 5 and bottom 5 schools based on overall passing rate, the average math score by grade level per school, the average reading score by grade level per school, and the scores by school spending per student, school size, and by school type. 

This information will be helpful to superintendents and the advisory board on how to distribute resources across all the different schools. The data was managed using Pandas, a Python library, that allows to easy data manipulation and visualization. We were able to use the Pandas library to clean up the data, change the structure of the data, and organize it into easy visualizations for the advisory board. 

## Results 

### 1. How is the district summary affected? 
 In the screenshots below, the first snip is the original code run with the incorrect Thomas High School ninth-grade scores for math and reading. The second snip shows the results without the scores. The Average Math Score, Average Reading Score, % Passing Math, % Passing Reading, and % Overall Passing metrics were slightly affected when the scores were taken out. 
 
**Changes between the metrics:**
- Average Math Score from 79.0 to 78.9
- Average Reading Score remained flat at 81.9 
- % Passing Math from 75.0% to 74.8% 
- % Passing Reading from 85.8% to 85.7%
- % Overall Passing from 65.2% to 64.9%

Original Data:
 
<img width="707" alt="district_summary_1 " src="https://user-images.githubusercontent.com/67871338/90343932-26d0a680-dfe3-11ea-8fd1-452b09bd0b76.PNG">

Adjusted Data: 

<img width="699" alt="district_summary_2 " src="https://user-images.githubusercontent.com/67871338/90343934-29cb9700-dfe3-11ea-9cdf-74617d608bc1.PNG">
 
### 2. How is the school summary affected?
Like above, the first screenshot is the unaltered data and the second details our results without the ninth-grade scores. The information was only adjusted for Thomas High School, so we can see the metrics that changed are for that school line only. 

**Changes between the metrics for Thomas High School:**
- % Passing Math from 66.9% to 93.19%
- % Passing Reading from 69.7% to 97.0%
- % Overall Passing from 65.1% to 90.6% 

Original Data: 

<img width="725" alt="school_summary 1 PNG" src="https://user-images.githubusercontent.com/67871338/90344341-f3901680-dfe6-11ea-8dae-b97396442dc5.PNG">

Adjusted Data: 

<img width="728" alt="school_summary 2 PNG" src="https://user-images.githubusercontent.com/67871338/90344347-f8ed6100-dfe6-11ea-9b25-503ff053e97b.PNG">

### 3. How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
By eliminating the ninth-grade scores, Thomas High School's math and reading performance increased. Relative to other schools, it increased its % Overall Passing from 65.1% to 90.6% and changed rank to # 2 overall in the school list. 

### 4. How does replacing the ninth-grade scores affect the following: 
####    - Math and reading scores by grade
For math and reading scores by grade, the only metrics affected are those for ninth-grade Thomas High School, which was the only area that was altered. These scores now show up as "nan" because they do not currently have scores. None of the other grades change because their data was not altered. 

**Math Scores By Grade:**

Original Data: 

<img width="230" alt="grades_per_school_1_math" src="https://user-images.githubusercontent.com/67871338/90344796-2c31ef00-dfeb-11ea-94ad-29d629636077.PNG">

Adjusted Data: 

<img width="232" alt="grades_per_school_2_math" src="https://user-images.githubusercontent.com/67871338/90344802-3522c080-dfeb-11ea-88eb-33dc5d75e25e.PNG">

**Reading Scores By Grade:** 

Original Data: 

<img width="231" alt="grades_per_school_1_reading" src="https://user-images.githubusercontent.com/67871338/90344819-48359080-dfeb-11ea-89f8-619f3fcaa174.PNG">

Adjusted Data: 

<img width="232" alt="grades_per_school_2_reading" src="https://user-images.githubusercontent.com/67871338/90344823-4a97ea80-dfeb-11ea-8646-5175c92a5bdc.PNG">

####    - Scores by school spending, school size, and school type
None of the metrics changed for the scores by school spending, school size, and school type. All of these stayed consistent with the information from the dataset before. 

## Summary 
In summary, the four major changes to the analysis after the reading and math scores were removed are: 

 1. % Passing Math 
 2. % Passing Reading 
 3. % Passing Overall 
 4. Rank of Thomas High School 
