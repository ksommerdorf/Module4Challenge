# PyCity Schools Analysis
## Overview of School District Analysis
The chief data scientist for a city school district, Maria, has asked for help in preparing all standardized test data for analysis, reporting, and presentation. The goal is to provide insights about performance trends and patterns to help make strategic decisions at the school and district level. The school board was recently notified that Thomas High School ninth graders' reading and math scores show evidence of academic dishonesty. This project is tasked to meet the goal by removing Thomas High School ninth graders' score data and analyzing the results.

## Development Environment
* Jupyter Notebook
* Python v3.10.4
  * Python Pandas library
  * Python Numpy library

## Resources
* [schools_complete.csv](https://github.com/ksommerdorf/Module4Challenge/files/8406366/schools_complete.csv)
* [students_complete.csv](https://github.com/ksommerdorf/Module4Challenge/files/8406370/students_complete.csv)

## Analysis Results
* District Summary
  * Original data:

![original_district_summary](https://user-images.githubusercontent.com/57520471/161465370-037ad1cc-c60e-4ba2-b5a5-42ce377bfa30.png)

  * Cleaned data:
 
![district_summary](https://user-images.githubusercontent.com/57520471/161465387-bfd09c9f-6d43-4185-98b4-5a687d1741a5.png)

  * The district summary data is mainly unaffected by the inaccurate data from Thomas High School. The only affect is the slight decrease (~0.1%) in the average math score, however this slight decrease is not significant enough to decrease the percentage of passing math.

* School Summary
  * Original data:
  
![original_school_summary](https://user-images.githubusercontent.com/57520471/161465895-1e6428f8-768a-448d-a9d5-d78aae02ddc9.png)

  * Cleaned data:
  
![school_summary](https://user-images.githubusercontent.com/57520471/161465486-8772201c-190e-4c31-ad12-12aa62b79737.png)

  * Thomas High School's overall percent passing rate decreased by ~0.3%. The percent passing reading when down ~0.3% and the percent passing math went down ~0.1%. The percent passing rate remains well over the average of the district of 65% at 90.6%.

* Thomas High School's Performance Compared to the Other Schools:
  * Original ranking:
  
![original_ranking](https://user-images.githubusercontent.com/57520471/161465518-f8b1bea4-c044-4951-a173-17f867861363.png)

  * After data cleaning ranking:
  
![new_ranking](https://user-images.githubusercontent.com/57520471/161465531-7043d6ce-ce3c-48b4-91b7-8d813dc5a450.png)

  * After replacing the ninth graders' math and reading scores, Thomas High School remains 2nd out of 14 schools in the district. 

* Math and Reading Scores by Grade:
  * Original data (math scores):
  
![original_math_scores](https://user-images.githubusercontent.com/57520471/161465541-72ae1eb9-1cc8-4370-b758-9a1b674691cf.png)
 
  * Cleaned data (math scores):
  
![math_scores](https://user-images.githubusercontent.com/57520471/161465563-ca113ab2-ef68-40ba-accf-519c36bdf40a.png)

  * The new average math score for ninth graders in Thomas High School is now not available. The other scores remain the same.
  
  * Original data (reading scores):
  
![original_reading_scores](https://user-images.githubusercontent.com/57520471/161465630-46ea8667-cc60-4b5d-b6fc-072881fa972a.png)

  * Cleaned data (reading scores):
  
![reading_scores](https://user-images.githubusercontent.com/57520471/161465654-e68435b0-2b03-4000-a127-35b46fa259d9.png)
 
  * The new average reading score for ninth graders in Thomas High Schools is also not available, all other scores remain the same. 

* Scores by School Spending:
  * Original data:
 
![original_school_spending](https://user-images.githubusercontent.com/57520471/161465685-4eb07233-2379-4f3e-ad24-6b5dc94a0013.png)
  
  * Cleaned data:
  
![school_spending](https://user-images.githubusercontent.com/57520471/161465726-c58ba443-0c7f-4f59-88a6-174fe4e0c4a2.png)
 
  * There is no effect on the original data of average scores by the amount spent per student. Both sets of data show a negative trend where as spending increases per student the overall passing percentage decreases.

* Scores by School Size:
  * Original data:
  
![original_school_size](https://user-images.githubusercontent.com/57520471/161465743-6e134617-2ad2-40c5-9b79-d65d90419193.png)
  
  * Cleaned data:
  
![school_size](https://user-images.githubusercontent.com/57520471/161465784-1560637f-2487-48fa-88ae-197d6fa9a04c.png)
  
  * There is no effect on the original data of score averages by school size. Both sets of data show a negative trend where as the size of the school increases the overall percent passing decreases.

* Scores by School Type:
  * Original data:
  
![original_school_type](https://user-images.githubusercontent.com/57520471/161465815-050fd2ba-16dc-4bd6-a2f8-96399338bb82.png)
  
  * Cleaned data:
 
![school_type](https://user-images.githubusercontent.com/57520471/161465828-b47991d6-3368-45ad-a6b2-b6a9938894e7.png)
  
  * There is no effect on the original data of score averages by school type. Both sets of data show a significant difference between charter school performance versus district school performance. Charter schools perform at a much higher rate with an overall passing percentage of 90% compared to district schools with an overall passing percent of 54%.

## Analysis Summary 
After cleaning the data by removing the ninth graders' reading and math scores from Thomas High School, only slight differences can be observed in the cleaned data. The differences are more noticeable at the school level because at the district level with a total of 39,170 students, 461 students is not as significant as compared to 1,635 students at Thomas High School. The noticeable changes include a ~0.1% decrease (83.42 to 83.35) in the average math scores, ~0.1% decrease (93.27 to 93.19%) in the percent passing math, ~0.15% decrease (83.85 to 83.90) in average reading score, ~0.3% decrease (97.31 to 97.02%) in percent passing reading, and ~0.3% decrease (90.95 to 90.63%) in percent overall passing. Therefore, the dishonest test scores did not significantly affect other schools in the district in comparison to Thomas High School but significantly affected the individual performance of Thomas High School. 
