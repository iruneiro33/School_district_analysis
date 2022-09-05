# School_district_analysis

## Overview of the school district analysis

This challenge analyzed data from an School District including math and reading grades, school funding, school type among other indicators. Howerver, there was evidence of academic dishonesty at the Thomas High School in the reading and math grades for the ninth graders. As such, it is important to replace those values and make adjustments to reflect the performance without the altered data. For this, we replace altered data with NaNs and run the whole analysis to see the effects it might hold to the School's performance.

## Results
This next section will answer specific questions with the analysis of the data obtained by running the file PyCitySchools_Challenge. 

* How is the district summary affected?
  When we remove the NaN values from the analysis, we see an overall declining perfomance in the following indicators: 
  
  ![Performance](https://user-images.githubusercontent.com/7553779/188344342-70aff628-42b3-4855-af92-4d268bedea1d.png)

Rounding up each percentage, the passing percentages changed to:
Math passing percentage declined to 75%
Reading passing percentage  decline to 86%
Tghe overall passing rate fell to 65%

* How is the school summary affected and how does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
  Specifically for the Thomas Hisgh school (THS), when the grades for the ninth grade are replaced with the NaN values we observe that: 
  
  ![THS_analysis](https://user-images.githubusercontent.com/7553779/188344926-c5006fb6-4f76-4dee-bf9f-c02e432c9b57.png)

  From the chart above we see that the THS falls to the bottom places. This is read as being one of the lowest performing schools of the district with passing percentages of :
  Math: 67%
  Reading: 70%
  Overall: 65%
  
  In adittion, if we analyze this results with other indicators such as spending, size and type we can see that the THS is also afected. 
  
 ## Addtional analysis
  
  * Analysis by Spending
  
  THS has a total number of 1635 students and a budget of	$1,043,130.00, with this it has an spending range (per student) of $631-$645. From the chart below, we can see that THS performance is below the average performance for the schools in the same range of spending. Even if this is only a benchmark indicator, the substitution of the 9th graders for the NaN values, altered their position from being an over-performing school in that spending range to an under-performing school, specifically in math and reading. The overall passing % is still within the range. 
  
  ![Spending_result_chart](https://user-images.githubusercontent.com/7553779/188347003-a1e667ed-580a-4f2b-8341-b89e2814a8b2.png)
  
   * Analysis by Size
   
  THS is considered a medium size school based on the number of student. The next chart shoes the performance of the school by size. Similarly, as the previous comparison, we observe that after the removal of the 9th graders, THS undeperforms in math and reading when compared to schoools of the similar size. Interesting enough, the middle size schools are the ones with the best performance of % passing in math, reading and overall.
  
  ![By_size](https://user-images.githubusercontent.com/7553779/188348556-9fad708c-a738-453c-a837-fd2f40ab7409.png)

  * Analysis by Type
     
  Finally, THS is a Charter School. Again we see the same behavior as before, going from over-performing to under-performing according to the benchmark by type of school. Howerver, on the overall passing percentage THS still has a greater result. This would be interesting to see, probably in this category there are over-performers or most of the bottom schools are Chartered. 

![By_type](https://user-images.githubusercontent.com/7553779/188348594-0f1bd9b8-a58b-436b-bf1d-a75a4f9ab419.png)
