# School_District_Analaysis

## Project Overview
A school board has asked us to analyze the data collected from fifteen schools along several metrics [grades, school size, district, math scores, reading scores, etc.]. Upon reviewing the data the school board noticed that there was academic dishonesty by one of their schools (Thomas High School's 9th grade class). They then requested to omit the reading and math score data from Thomas High School as to not affect the results and have asked to run the analysis again in order to track any changes. 

## Resources
- Data Source: students_complete.csv
- Software: Python 3.6.1
- Jupyter Notebook (anaconda3)
- Pandas 1.3.5
- Git Bash 2.37.1.windows.1

## Results
After removing Thomas High School's reading and math scores, the results from the analysis show that:
- There was little to no change in the district summary.
  - Original '% Overall Passing': 65.2%
  - Adjusted '% Overall Passing': 64.9%
      - This result falls within expectation as the population of Thomas High School ninth-graders was only 461 students (1.18%) of the total 39,170 students across the entire district. There's an argument to be made that it would be more surprising if there was a more significant change as that could indicate something else amiss with the data.
      
- There was significant change in the school summary of Thomas High School
  - Original 'Thomas High School' '% Overall Passing': 90.94%
  - Adjusted 'Thomas High School' '% Overall Passing': 65.08% 
    - This is a significant change in performance for Thomas High School now that the data has been adjusted to reflect the remaining population of 10th-12th graders. Although they are no longer the second highest performing school, they are still ranked in the middle at 8th [of 15]. 
 
- Removing the ninth-graders scores resulted in the following minor changes:
  - Math (by grade)
    - Original 'Ninth Grade Math Scores': 80.35%
    - Adjusted 'Ninth Grade Math Scores': 80.12%
  - Reading (by grade)
    - Original 'Ninth Grade Reading Scores': 82.51%
    - Adjusted 'Ninth Grade Reading Scores': 82.42%  
  - Scores by School Type
    - Original 'Charter' '% Overall Passing': 90.43%
    - Adjusted 'Charter' '% Overall Passing': 90.39%
    
      - Original 'Charter' '% Passing Math': 93.62%
      - Adjusted 'Charter' '% Passing Math': 93.61%
      
      - Original 'Charter' '% Passing Reading': 96.58%
      - Adjusted 'Charter' '% Passing Reading': 96.55%  

- Removing the ninth-graders scores resulted in no changes in the following:
  - school spending
  - school size
  - scores in grades 10th-12th were unaffected

  
## Summary
- Removing the scores of 9th graders from Thomas High School had little effect on the resulting holistic data we aggregated from across these fifteen schools: district summary, ninth grade math scores, ninth grade reading scores, and scores by school type (specifically charter). The only significant changes could be seen within Thomas High School's data in reading and math scores of the remaining 10th-12th grade population. 
