# Analysis of School District Data: Math and Reading Scores of Students

For this part of the Challenge, write a report that summarizes your updated analysis and compares it with the results from the module.

## Overview of the school district analysis

We have analyzed math and reading scores for a school district that included 39170 students in 15 schools. We have calculated average math scores, average reading scores, passing math scores, passing reading scores, overall passing scores, and percentages of XX. A number of programming tools (for working with Pandas data analysis library and NumPy) were used that included data import, merging data frames and data series, conditionals, mathematical calculations, and indexing.   

However, the school board had identified an academic dishonesty from the data, especially in the 9th graders of the Thomas High School (THS) and decided to drop all math and reading scores of 9th graders at the THS. The school district analysis was repeated to see how these changes affected the overall analysis. For this task, we have used .loc function in pandas to locate math and reading scores of 9th graders at the ths, and used np.nan method to remove grades.

Software tools: Pandas, Git

2. Results: Using bulleted lists and images of DataFrames as support, address the following questions.
Reading and math scores were removed from 9th graders at the THS, and the following data frame depicts that.

    - How is the district summary affected?
      
      - Reduced by a small amount (average score by ~ 0.1) or percentage (by ~ 0.2%)

    - How is the school summary affected?
It dropped by ~0.05-0.06% foe scores and passing percentages dropped by ~27% for passing scores. This is because 9th graders at ths have no grades.
    1635	$1,043,130.00	$638.00	83.418349	83.848930	93.272171	97.308869	90.948012	$631-645
    1635	$1,043,130.00	$638.00	83.350937	83.896082	66.911315	69.663609	65.076453
    
    - How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
    It increased.
    
    - How does replacing the ninth-grade scores affect the following:
      - Math and reading scores by grade
      
      - Scores by school spending
      No change
      
      - Scores by school size
      Medium size schools changed (increased) by ~ 0.01 and decreased passing grades by ~0.01%
      
      - Scores by school type
      Changed by ~ xx for scores and xx for passing
3. Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

- Deliverable 3 Requirements

- Structure, Organization, and Formatting (7 points)

- The written analysis has the following structure, organization, and formatting:

There is a title, and there are multiple sections (2 pt).
Each section has a heading and subheading (3 pt).
Links to images are working, and code is formatted and displayed correctly (2 pt).
Analysis (18 points)

The written analysis has the following:

- Overview of the school district analysis:

  - The purpose of this analysis is well defined (3 pt).

- Results:

  - There is a bulleted list that addresses how each of the seven school district metrics was affected by the changes in the data (10 pt).

- Summary:

  - There is a statement summarizing four changes to the school district analysis after reading and math scores have been replaced (5 pt).
Submission

Once you’re ready to submit, make sure to check your work against the rubric to ensure you are meeting the requirements for this Challenge one final time. It’s easy to overlook items when you’re in the zone!

As a reminder, the deliverables for this Challenge are as follows:

- Deliverable 1: Replace ninth-grade reading and math scores
- Deliverable 2: Repeat the school district analysis
- Deliverable 3: A written report for the school district analysis (README.md)

Upload the following to your School_District_Analysis GitHub repository:

- The PyCitySchools_Challenge.ipynb file.
- The Resources folder with the schools_complete.csv and students_complete.csv files.
- An updated README.md that has your written analysis.

