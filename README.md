# **PyCitySchools with Pandas**
	
## **Overview of School District Analysis** 
* Maria, chief Data scientist for a city School district is tasked with preparing all standardized test data for analysis, reporting and presentation to provide trends about performing trends and patterns. we will be helping Maria by analyzing the school district data(student funding data and student's standardized test scores) to showcase trends in school performance. We will complete the following tasks
	* Generate District Summary table 
	* Generate School Summary table
	* Tables presenting each of the following metrics:
		* Top 5 and bottom 5 performing schools, based on the 			overall passing rate
		* The average math and reading score received by 	grade 		level at each school
		* Group Scores by School Spending per Student
		* Group Scores by School Size
		* School performance based on the type of school
* This Analysis will assist the school board in making decisions regarding the school budget and priorities.
 
### Purpose 
* To replace the math and reading scores for ninth grade of Thomas High School with `NaNs` while keeping the rest of the data intact. Then repeat the school district analysis that we did in this module using the new math and reading data. As well to create a summary report based on the analysis and finding of the school district data and how the changes on school data affected the overall analysis.


## **Results** 

![District summary df with updated Thomas 9th grade data](C:/Users/Ruth/OneDrive/Desktop/Class_Work/Module_4/HW4_Submission_Pandas/Resources/district_summary_df1.png) 

![District summary df in the module](C:/Users/Ruth/OneDrive/Desktop/Class_Work/Module_4/HW_Submission_Pandas/Resources/district_summary_dfmodule.png) 

* How is the district summary affected?
	* we can see from the images above, that the updated district summary results are slightly lower than the results in the module. Average Math Score (is 78.9 in the updated table and 79.0 in the module), Average Reading Score (is same 81.9 in both tables), `% Passing Math` (is 74.8 in the updated table and 75.0 in the module), `% Passing Reading` (is 85.7 in the updated table and 85.8 in the module), `% Overall Passing` (is 64.9 in the updated table and 65.2 in the module). The updated district summary results are approximately (0.1, 0, 0.2, 0.1, 0.3) respectively lower than the results in the module. Total schools, Total students and Total budget are same. The math and reading scores for Thomas high school 9th grade has been replaced with Nans. We used the new total student count without Thomas High School ninth_grade students to recalculate the passing math and passing reading percentages, and the overall passing percentage. 

![School summary df with updated Thomas 9th grade data](C:/Users/Ruth/OneDrive/Desktop/Class_Work/Module_4/HW4_Submission_Pandas/Resources/per_school_summary_df.png)

![School summary df in the module](C:/Users/Ruth/OneDrive/Desktop/Class_Work/Module_4/HW4_Submission_Pandas/Resources/per_school_summary_dfmod.png) 
 
* How is the school summary affected?
	* The results for all the schools are same in both the updated table and in the module. As you can see from the images above, for Thomas high school some of the results in the new table are slightly lower than the one in the module. Average Math Score (is 83.4 in the updated table and 83.4 in the module), Average Reading Score (is 83.9 in the updated table and 83.8 in the module), `% Passing Math` (is 93.2 in the updated table and 93.3 in the module), `% Passing Reading` (is 97 in the updated table and 97.3 in the module), `% Overall Passing` (is 90.6 in the updated table and 90.9 in the module). The updated School summary results for Thomas high school for Average Math Score, `% Passing Math`, `% Passing Reading` and `% Overall Passing` are approximately (0, 0.1, 0.3, 0.3) respectively lower than the results in the module. Only Average Reading Score for Thomas is slightly higher in the updated table than the scores in the module by (0.1). For Thomas high school, we recalculated the percentage of students who passed math, passed reading, and passed both math and reading using 10th grade to 12th grade total and data of Thomas High school only and added it to the table.  

![The top 5 performing schools after replacing Thomas 9th grade data](C:/Users/Ruth/OneDrive/Desktop/Class_Work/Module_4/HW4_Submission_Pandas/Resources/top_schools_dfnew.png) 

![The top 5 performing schools in the module](C:/Users/Ruth/OneDrive/Desktop/Class_Work/Module_4/HW4_Submission_Pandas/Resources/top_schools_df.png) 
	
* How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
	* The image above shows the 5 top performing schools based on the overall passing rate with the updated data and in the module. Thomas high school has “overall passing percentage” of `90.6` in the updated table and `90.9` in the module (second Table). It is in the 2nd place in both tables. So, its performance relative to other schools did not change even though the overall passing percentage is slightly lower in the updated table (where ninth graders' math and reading scores have been replaced). 

* How does replacing the ninth-grade scores affect the following:
![math_scores_by_grade after replacing Thomas 9th grade data](C:/Users/Ruth/OneDrive/Desktop/Class_Work/Module_4/HW4_Submission_Pandas/Resources/math_scores_by_gradenew.png)
 
![math_scores_by_grade in the module](C:/Users/Ruth/OneDrive/Desktop/Class_Work/Module_4/HW4_Submission_Pandas/Resources/math_scores_by_gradmod.png)

 ![reading_scores_by_grade after replacing Thomas 9th grade data](C:/Users/Ruth/OneDrive/Desktop/Class_Work/Module_4/HW4_Submission_Pandas/Resources/reading_scores_by_gradenew.png)

	* Math and reading scores by grade
		* The math and reading scores by grade for the ninth grade of Thomas high school show as Nans in the updated DataFrames and "83.6"(for math) and "83.7"(for reading) in original analysis of the module.  The 10th, 11 th and 12th grades of Thomas High School and all the grades of the other schools, their math and reading scores have not changed.

![Scores by school spending after replacing Thomas 9th grade data](C:/Users/Ruth/OneDrive/Desktop/Class_Work/Module_4/HW4_Submission_Pandas/Resources/spending_summary_dfnew.png) 

![Scores by school spending_summary in the module](C:/Users/Ruth/OneDrive/Desktop/Class_Work/Module_4/HW4_Submission_Pandas/Resources/spending_summary_dfmod.png) 	
	* Scores by school spending
		* As you can see from the images above, all scores by school spending are same in the table with updated data and in the table of the module. So, replacing Thomas high school ninth grade scores by Nans for math and reading does not affect the scores by school spending.

![Scores by School size after replacing Thomas 9th grade data](C:/Users/Ruth/OneDrive/Desktop/Class_Work/Module_4/HW4_Submission_Pandas/Resources/size_summary_dfnew.png) 

![Scores by School size in the module](C:/Users/Ruth/OneDrive/Desktop/Class_Work/Module_4/HW4_Submission_Pandas/Resources/size_summary_dfmod.png) 	
	* Scores by school size
		* As you can see from the images above, all scores by school Size are same in the table with updated data and and in the table of the module. So, replacing Thomas high school ninth-grade scores by Nans for math and reading does not have an effect on scores by school size.
![Scores by School type after replacing Thomas 9th grade data](C:/Users/Ruth/OneDrive/Desktop/Class_Work/Module_4/HW4_Submission_Pandas/Resources/type_summary_dfnew.png) 

![Scores by School type in the module](C:/Users/Ruth/OneDrive/Desktop/Class_Work/Module_4/HW4_Submission_Pandas/Resources/type_summary_dfmod.png) 	
	* Scores by school type
		* As you can see from the images above, all scores by school Type are same in the table with updated data and in the table of the module. So, replacing Thomas high school ninth-grade scores by Nans for math and reading does not have an effect on scores by school type.

## **Summary** 
* four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs are.

	* The school district summary table shows slightly lower scores (for Average Math Score, the passing math and passing reading percentages, and the overall passing percentage) by approximately (0.1-0.3) than the school district summary in the module.

	* The overall passing percentage Of Thomas High School has changed from 90.9 in the original analysis to 90.6 updated school district analysis. This did not affect its performance; it is one of the top performing schools.

	* In the School summary table, Thomas High school scores for(Average Math Score, the passing math and passing reading percentages, and the overall passing percentage) are slightly lower by approximately (0.1-0.3) than the scores in the original analysis of the module. Only Average Reading Score for Thomas is slightly higher in the updated table than the scores in the module by (0.1).

	* In the Math and reading scores by grade table of the updated Analysis, the ninth grade score for Thomas High School shows as NaNs. It has changed from "83.6"(for math) and "83.7"(for reading) in the original Analysis to NaNs in the Updated Analysis.

* Even though Thomas High school ninth grade scores for math and reading scores have changed to Nans, the school is still in the second place of the 5 top performing schools. This change has minimum affect to its performance.

