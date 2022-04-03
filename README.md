# Analysis of School District Data: Math and Reading Scores of Students

For this part of the Challenge, write a report that summarizes your updated analysis and compares it with the results from the module.

## Overview of the school district analysis

We have analyzed math and reading scores for a school district that included 39170 students in 15 schools. We have calculated average math scores, average reading scores, passing math scores, passing reading scores, overall passing scores, and percentages of XX. A number of programming tools (for working with Pandas data analysis library and NumPy) were used that included data import, merging data frames and data series, conditionals, mathematical calculations, and indexing.   

However, the school board had found evidence of academic dishonesty from the data (specifically, reading and math grades for Thomas High School ninth graders appear to have been altered). . The school board wanted to want to uphold state-testing standards and decided to drop all math and reading scores of 9th graders at the THS while keeping other data intact. Therefore, the school district analysis was repeated to see how these changes affected the overall analysis. For this task, we have used .loc function in pandas to locate math and reading scores of 9th graders at the THS, and used np.nan method to remove grades.

Software tools: Pandas, Git

## Results: Using bulleted lists and images of DataFrames as support, address the following questions.

Reading and math scores were removed from 9th graders at the THS, and the Figure 1 below shows the removal of data (a portion is shown) of 9th graders at the THS.

  ![School DataFrame](/resources/school_data_after_removing_grades.png)
   
  ### Figure 1. Screenshot of Notebook showing Student Data for NAN and a Summary of Dataset
  
  There were 461 ninth graders (39170 - 38709) at the THS whose math and reading scores were removed from the analysis. 
  
  - How is the district summary affected?
      - Reduced by a small amount (average score by ~ 0.1) or percentage (by ~ 0.2%). However, it was not sigficant to the whole number. See Figure 2 below.


![District Summary Before](/resources/district-summary-before.png)

![District Summary After](/resources/district_summary_after_repeating.png)
 

### Figure 2. District Summary Before and After Removing Grades


- How is the school summary affected?

  - For Thomas High School, scores were dropped by ~0.05-0.06% and passing percentages were dropped by ~27% (See Figure 3A (before) and Figure 3B (after removing grades). This is because 9th graders at ths have no grades. After re-calculating 10th-12th graders for the THS, the percentages were increased again (Figure 3C) Scores were not affected for other schools. 
    
    ### 3A
  ![School Summary Before Repeating](/resources/school_summary_before-repeating.png)
  
   ### 3B
  
  ![School Summary After_Removing_9thGr](/resources/school_summary-after-removing-9thgr.png)
  
   ### 3C
   
  ![School Summary After_Recalculating_THS-10TH-12TH](/resources/school-summary-after-including_THS10th-12th.png)
  
- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
   
  - It decreased passing percentages. 

- How does replacing the ninth-grade scores affect the following:

  - Math and reading scores by grade

  All schools had a grade EXCEPT for THS 9th graders
      
  ![math-score-by-grade-before](/resources/math-scores-by-grade-before.png)
  
  ![math-score-by-grade-after](/resources/math-scores-by-grade-after.png)
  
  ![reading-score-by-grade-before](/resources/reading-scores-by-grade-before.png)
  
  ![reading-score-by-grade-after](/resources/reading-scores-by-grade-after.png)
  
  - Scores by school spending
      No change
  ![spending-before](/resources/spending-before.png)
  
  ![spending-after](/resources/spending-after.png)
      
      
  - Scores by school size
      Medium size schools changed (increased) by ~ 0.01 and decreased passing grades by ~0.01%
      
![school-size-before](/resources/school-size-before.png)
![school-size-after](/resources/school-size-after.png)

      
  - Scores by school type
      Changed by ~ xx for scores and xx for passing
      
 ![school-type-before](/resources/school-type-before.png)
 
 ![school-type-after](/resources/school-type-after.png)
      
## Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.


The link to the Notebook: [PyCitySchools_Challenge](/PyCitySchools_Challenge.ipynb)
