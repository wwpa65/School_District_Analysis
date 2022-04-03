# Analysis of School District Data: Math and Reading Scores of Students

## Overview

We have analyzed math and reading scores for a school district that included 39170 students in 15 schools. We have calculated average math scores, average reading scores, passing math scores, passing reading scores, overall passing scores, and percentages of XX. A number of programming tools (for working with Pandas data analysis library and NumPy) were used that included data import, merging data frames and data series, conditionals, mathematical calculations, and indexing.   

However, the school board had found evidence of academic dishonesty from the data (specifically, reading and math grades for Thomas High School ninth graders appear to have been altered). . The school board wanted to want to uphold state-testing standards and decided to drop all math and reading scores of 9th graders at the THS while keeping other data intact. Therefore, the school district analysis was repeated to see how these changes affected the overall analysis. For this task, we have used .loc function in pandas to locate math and reading scores of 9th graders at the THS, and used np.nan method to remove grades.

Software tools: Pandas, Git

## Results

Reading and math scores were removed from 9th graders at the THS, and the Figure 1 below shows the removal of data (a portion is shown) of 9th graders at the THS.

  ![School DataFrame](/resources/school_data_after_removing_grades.png)
   
  ### Figure 1. Screenshot of notebook showing student data for NAN and a summary of dataframe
  
  There were 461 ninth graders (39170 - 38709) at the THS whose math and reading scores were removed from the analysis. 
  
## 1. How is the district summary affected?

      - There was a very minute change in scores for some, however, it was not sigficant to the whole number. See Figure 2 below.

### 1A (Before replacement)
![District Summary Before](/resources/district-summary-before.png)

### 1B (After)
![District Summary After](/resources/district_summary_after_repeating.png)
 

### Figure 2. District summary before and after removing scores of 9th graders at THS


## 2. How is the school summary affected?

  - For Thomas High School, scores were not much affected. Math, reading, and overall and passing percentages were dropped by ~26% (See **Figure 3A** (before) and **Figure 3B** (after removing grades). 
  - This is because 9th graders at THS have no grades. After re-calculating 10th-12th graders for the THS, the passing percentages were increased again (**Figure 3C**) 
  - Scores were not affected for other schools. 
    
    ### 3A (Before replacement)
  ![School Summary Before Repeating](/resources/school_summary_before-repeating.png)
  
   ### 3B (After replacement)
  
  ![School Summary After_Removing_9thGr](/resources/school_summary-after-removing-9thgr.png)
  
   ### 3C (After replacement and recalculating 10-12th grade)
   
  ![School Summary After_Recalculating_THS-10TH-12TH](/resources/school-summary-after-including_THS10th-12th.png)
  
  ### Figure 3. School summary before (3A), after removing 9th grades for THS (3B), and after recalculating for 10th-12th graders for THS (3C)
  
  
## 3. How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
   
  - It decreased passing percentages of Thomas High School (See Figure 3A and 3B above under Thomas High School). 

## 4. How does replacing the ninth-grade scores affect the following:

  - **Math and reading scores by grade**

  All schools had math and reading scores EXCEPT for 9th graders at Thomas High School (see Figure 4).
   
   ## A (math - before replacement)
  ![math-score-by-grade-before](/resources/math-scores-by-grade-before.png)
  
  ## B (math - after replacement)
  ![math-score-by-grade-after](/resources/math-scores-by-grade-after.png)
  
  ## C (reading - before replacement)
  ![reading-score-by-grade-before](/resources/reading-scores-by-grade-before.png)
  
  ## D (reading - after replacement)
  ![reading-score-by-grade-after](/resources/reading-scores-by-grade-after.png)
  
  ### Figure 4. Math and reading scores by grade for schools before (A, C) and after (B, D) replacing scores
  
  - **Scores by school spending**
    - There was no effect on school spending 
  
  ### Before replacement
  ![spending-before](/resources/spending-before.png)
  
  ### Before replacement
  ![spending-after](/resources/spending-after.png)
      
      
  - **Scores by school size**
    - There was no effect on the scores by size
      
![school-size-before](/resources/school-size-before.png)

![school-size-after](/resources/school-size-after.png)

      
  - Scores by school type
 
 Score by school type did not change before and after (the final scores), It may be probably because the scores were recalculcated using ONLY 10th-12th graders of THS.  
      
 ![school-type-before](/resources/school-type-before.png)
 
 ![school-type-after](/resources/school-type-after.png)
      
## Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

1. Math and reading scores of 461 9th grade students at Thomas High Schoolwere removed from grading
2. Percentage passing math for Thomas High School was dropped by ~26%
3. Percentage passing reading  reading for Thomas High School was dropped by ~27%
4. Percentage passing math and reading for Thomas High School was dropped by ~26%


The link to the Notebook: [PyCitySchools_Challenge](/PyCitySchools_Challenge.ipynb)
