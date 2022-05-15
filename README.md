# School District Analysis

## Overview and Purpose
After submitting school district analyses examining academic metrics (reading and math scores and passing percentages on a district basis, and then by individual schools, grade, spending per student, school size, and school type), we were notified that 9th graders at Thomas High School may have been involved in academic dishonesty with altered standardized testing scores. As a result, Maria has requested that repeat the same analyses but ignore the scores from the 9th graders at Thomas High School. To effect this, we replaced all math and reading scores from Thomas High Schools with NaN (not a number) while leaving the rest of the data the unchanged. The original and revised analyses included:
-	A district summary 
-	A school summary 
-	The top five performing schools, based on the overall passing rate
-	The bottom five performing schools, based on the overall passing rate
-	The average math score by grade for each school
-	The average reading score by grade level for each school
-	An examination of the metrics by school spending per student
-	An examination of the metrics by school size
-	An examination of the metrics by school type

## Resources
-	Data Source: schools_complete.csv, students_complete.csv
-	Software: Jupyter Notebooks, conda 4.12.0, Python 3.7.2

## Results
For results, we compared the original summaries that included math and reading scores for Thomas High School 9th graders with the revised ones that replaced those scores with NaN.
-	The revised district summary reflected changes in the Average Math Score, % Passing Math, % Passing Reading, and % Overall Passing. The revised analysis shows:
    -	Average Math Score decreased from 79 to 78.9
    -	% Passing Math decreased from 75 to 74.8 
    -	% Passing Reading decreased from 85.8 to 85.7
    -	% Overall Passing decreased from 65.2 to 64.9

Original District Summary

![Original_district_summary_df](https://user-images.githubusercontent.com/101822948/168480859-10c4f85c-14ff-4773-81df-73febf16e291.png)

Revised District Summary

![Revised_District_Summary](https://user-images.githubusercontent.com/101822948/168480864-f8fe97cf-80d6-4b67-ab1b-5b26d8c1175a.png)

- The academic metrics of Thomas High School showed a notable change after 9th grade scores were omitted. All of its metrics reflected a decrease from the original analysis, except for the average reading score, which increased.  

Original Per School Summary

![Original_per_school_summary_df](https://user-images.githubusercontent.com/101822948/168481011-e5c55c57-454f-4b59-a373-4a94bb2885fe.png)

Revised Per School Summary

![Revised_Per_School_Summary](https://user-images.githubusercontent.com/101822948/168480962-d405c278-d354-4a04-9599-edebb96282ef.png)

-	Replacing Thomas High School 9th graders had little impact on its performance relative to other schools. In the original analysis Thomas High School ranked second in top performing schools. The revised analysis reflected the changes noted above for the school, but the difference was so marginal that it did not impact the rankings.  

Original Top 5 Schools

![Original_top_5_school](https://user-images.githubusercontent.com/101822948/168481052-d2d678cb-531c-470d-8487-ebaf3a00afdc.png)

Revised Top 5 Schools

![Revised_Top_Schools](https://user-images.githubusercontent.com/101822948/168481124-63173a2f-7e2f-41c0-8899-eb092523bed1.png)

-	In the revised analyses, by replacing the 9th graders’ scores at Thomas High School the following results indicated:
  - In the analyses for Average Math and Reading Scores by grade, the scores for Thomas High School clearly show NaN, which provides useful information to the district. It lets them clearly know that the scores were excluded and did not impact the results for the other grades at Thomas High School.
 
Revised Math Scores

![Revised_Math_Scores_by_Grade](https://user-images.githubusercontent.com/101822948/168481230-8053c67e-2a32-454f-b0f0-21767293f08e.png)

   -	In the analysis for scores by school spending we calculated the per student budget for each school and placed the schools into bins based on their spending per school, which could provide valuable information to the district in regards to where to allocate future funding. The revised analysis did not impact the spending per student at any school, but if evidence of tampering with scores is proven then the school district could also make punitive decisions against Thomas High School, which receives around $638/student.

Original Spending Range Per Student
  
 ![Original_spending_range_per_student](https://user-images.githubusercontent.com/101822948/168481161-eb6a1ea1-20b9-4769-b55d-0fb445db58f4.png)
 
  
   -	In the analysis for scores by school size, we made bins based on the total students in each school. The impact of the revised analysis had little impact on school size because even though the scores of the 9th graders were omitted, they still contribute to the school population. 
  
School by Size summary between the two reports also appeared identical after both analyses when metrics were rounded to the first decimal. 
  
  ![Revised_School_Size](https://user-images.githubusercontent.com/101822948/168481416-647b6d9d-f2e5-44fa-ab7c-340538d60cbb.png)

   - In the analysis for scores by type, the revised analysis also did not show any major difference. However, the school district could request more oversight into charter schools if evidence of cheating is proven or even close down a school, so this data could change in the future. 

Both the original and revised School by Type summaries yielded these results: 

![original_school_size](https://user-images.githubusercontent.com/101822948/168489259-afa747ea-c716-40c1-9bbb-c2d9941512a4.png)


## Summary 
After running the new analysis, there were several notable changes to the revised School District Analysis after we replaced the student scores of Thomas High School 9th graders with NaN. 
-	The Average Math Score decreased by 1/10 of a point from 79 to 78.9
-	The Average Reading Score remained unchanged at 81.9
-	The % Passing Math decreased by .2% to 74.8%, down from 75%.
-	The % Passing Reading decreased .1% to 85.7%, down from 85.8%
-	% Overall Passing decreased .3% to 64.9%, down from 65.2%

## Conclusion
If Thomas High School intentionally altered their 9th graders reading and math scores, the impacts benefited not only the school, but also the districts’ metrics. However, omitting their results and updating the analysis is the correct action in order to maintain integrity at the district. The school board may want to use the analysis to make budget changes or increase oversight at Thomas High School. 
