# School_District_Analysis
Resources: Python 3.7.7; Conda 4.7.12

## Challenge Overview
1. Correct the students' names so there are no professional prefixes or suffixes. (This was taken into account in Cell 9-10)
2. Replace the reading and math scores for ninth graders at Thomas High School with NaN. (The following analysis begin after a cell with import numpy as np)
3. Merge the clean student data with the school dataset.
4. Present a written analysis that correctly answers the following questions: 
- How is the district summary affected?
- How is the school summary affected?
- How does removing the ninth graders' math and reading scores affect Thomas High School's performance, relative to the other schools?
- How does removing the ninth grade scores affect the following?
    - Math and Reading Scores by Grade
    - Scores by School Spending
    - Scores by School Size
    - Scores by School Type

## Challenge Summary
The analysis of the PyCitySchools data show:
- The district summary was affected by a non-significant difference in Average Math Score, % Passing Math, % Passing Reading, and % Overall Passing.
    - Refer to: new_district_summary_df
    ![](pictures/District%20summary.png)
- The school summary was affected the number of students who passed math, reading, and both math and reading by returning less number of students. This result reduced % Passing Math, % Passing Reading, and % Overall Passing for Thomas High School only. The NaN values in math and reading scores for Thomas High School 9th graders did not affect any other schools' performances.
    - Refer to: new_per_school_summary_df
- Removing the ninth graders' math and reading scores shifted Thomas High School from ranking 2nd highest performing group to ranking the middle performing group out of 15 schools. 
    - Refer to: new_top_schools
- Removing the ninth grade scores only affected scores of Thomas High School ninth graders as it returned values of NaN for both math and reading. 
    - Refer to: new_math_scores_by_grade and new_reading_scores_by_grade
- Removing the ninth grade scores reduced the average % Passing Math, average % Passing Reading, and average % Overall Passing of the schools in the 3rd range of spending ($630-644). 
    - Refer to: new_spending_summary_df
    ![](pictures/Scores%20by%20spending.png)
- Removing the ninth grade scores affected the medium size (1000-2000) schools by reducing the average % Passing Math, average % Passing Reading, and average % Overall Passing. 
    - Refer to: new_size_summary_df
    ![](pictures/Scores%20by%20size.png)
- Removing the ninth grade scores affected the Charter schools by reducing the average % Passing Math, average % Passing Reading, and average % Overall Passing. 
    - Refer to: new_type_summary_df
    ![](pictures/Scores%20by%20type.png)
