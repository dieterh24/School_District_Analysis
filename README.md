# School_District_Analysis
1.	Overview of the school district analysis: Explain the purpose of this analysis.
The purpose of this task is to provide insights to a district school board.  The initial purpose was to analyze the data across 15 schools within this district to determine overall math and readings scores and percentages within the district.  The board wanted to review those results, plus look at size (number or students), and their respective budgets (per student).  The school board found evidence of cheating at Thomas High School (THS), in the ninth grade, for both reading and math scores.  The analysis was pivoted to exclude THS data scores to evaluate the data between the two sets of data.     
2.	Results: Using bulleted lists and images of DataFrames as support, address the following questions.
How is the district summary affected?  Nominal impact, total schools and budget data were not impacted.  The scores declined slightly with the average reading score remaining unchanged.
PyCitySchools District Summary								
Description	Total School	Total Students	Total Budget	Avg Math Score	Avg Reading Score	% Passing Math	% Passing Reading	% Overall Passing
All data	15	                  38,709 	 $  24,649,428.00 	79.0	81.9	75.0%	85.8%	65.2%
Exclude THS scores 9th grade scores	15	                  39,170 	 $  24,649,428.00 	78.9	81.9	74.8%	85.7%	64.9%

How is the school summary affected?  We took out 461 9th graders to get 1,174 students at THS.  The average math score remained the same, & the average reading score went down by .01.  The overall scores went down by .03.  
Thomas High School 	School Type	Total Students	Total Budget	Per student budget	Avg Math Score	Avg Reading Score	% Passing Math	% Passing Reading	% Overall Passing
Before	Charter	                     1,635 	 $    1,043,130.00 	 $          638.00 	83.4	83.8	93.3%	97.3%	90.9%
After	Charter	                     1,174 	 $    1,043,130.00 	 $          888.53 	83.4	83.9	93.2%	97.0%	90.6%

How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?  Pulling one grade from one high school didn’t impact much overall.  
How does replacing the ninth-grade scores affect the following:  
Math and reading scores by grade:  Maria should note that all grades run at about the same percentage in grades with little deviation between the scores for math and reading within a school.
Scores by school spending:  there are slight changes in most values removing the students, the biggest delta is the per student spend going from $638 to ~$888 per.  Total budget for the school did not change, so taking out the 461 students resulting in the increase per.
Scores by school size:  School size is remains medium as they are still over 1,000 students at THS.
Scores by school type:  Charter schools score higher that district schools.  We count conclude that THS 9th grade students received similar grades to others in charter schools (same grade).
3.	Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
a.the biggest change was in the spending per student measurement after moving the 9th graders from the overall measure.
b.removing the 461 students skews the dollars, and it puts THS as an outlier when you review the per student spend vs. other schools in the district.  
c.THS is now tied for second when looking at the overall % for schools vs. being in second place alone, but as mentioned, the big change was the budget per student.
d.the decrease in scores after pulling out the 9th graders from THS is nominal, and not a huge impact to the overall scores (they did not fluctuate much).  It’s a fair assumption that the 9th graders at THD scores similar to other 9th graders within the charter school population.  
