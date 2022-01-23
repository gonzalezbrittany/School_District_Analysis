# School_District_Analysis

## Overview

The Chief data scientist for the city school districts is looking into student funding and standardized test scores for reading and math. She is interested in finding out if there are variables that had influenced the outcomes of the school districts standardize test scores. 

For this analysis we initially performed the following calculations:
* Calculate the number of schools
* Calculate the total number of students
* Calculate the total budget
* Calculate the average math and reading scores
* Calculate the percentage of students that passed math 
* Calculate the percentage of students that passed reading
* Calculate the percentage of students that passed both math and reading.

A DataFrame was created to display the findings 
![image](https://user-images.githubusercontent.com/26393180/150690875-50a46447-b3d5-4fdd-9fbb-286cb3d963e5.png)

Per request, additional calculations were peformed and are presented below.

* Break down the previously calculated data by school. The school type was added to the DataFrame per request.
![image](https://user-images.githubusercontent.com/26393180/150690942-206808c5-82a2-46c0-840b-f4d3e7b5a41e.png)

* The top five scoring schools presented in a DataFrame
![image](https://user-images.githubusercontent.com/26393180/150690993-73095304-e43d-417f-839f-1232f0cd4e36.png)

* The lowest five scoring schools presented in a DataFrame
![image](https://user-images.githubusercontent.com/26393180/150691022-7a0e41cc-cecd-4b15-bd09-17d78fe0d423.png)

* Average scores for both reading and math were presenting in two separate Data frames. 
![image](https://user-images.githubusercontent.com/26393180/150691081-fd59f6df-88fd-4d01-8f60-2b5d9680fb4b.png)

* Ranges were created to find the average scores based on the spending range per student
![image](https://user-images.githubusercontent.com/26393180/150691093-94a9a887-e2e7-4ae1-8e64-9adc996e1b2d.png)

* The average math and reading calculation were broken down by school size
![image](https://user-images.githubusercontent.com/26393180/150691110-af0823b5-367a-4298-b9d0-f9fec9aa4c3e.png)

* The average math and reading calculations were broken down by school type
![image](https://user-images.githubusercontent.com/26393180/150691128-0d81cfba-5f90-49d6-bcd7-1fed69791a48.png)

After the initial calculations were completed, it was discovered that there may have been academic dishonesty with the reading and math grades for Thomas High Schools ninth graders. The grades appeared to have been altered. After the discovery, the math and reading scores for Thomas High Schools ninth graders were removed from the initial dataset. The analysis was then redone to see if there were any differences between the initial results and the results after Thomas High Schools ninth graders test scores were removed. 

## Resources
Data Source: schools_complete.csv , students_completed.csv
Software: Python 3.6.1, Jupyter Notebook

## Re-analysis and Comparison Results

The following questions were addressed after the re-analysis was complete

*	How was the district summary affected?

Initial results
![image](https://user-images.githubusercontent.com/26393180/150691281-ec21a1b3-4f89-4dbb-90aa-2b166eba1ae8.png)

Recalculated results
![image](https://user-images.githubusercontent.com/26393180/150691287-910ebdad-732b-48b8-9aee-c7ffed076251.png)
When comparing the initial and recalculated district summary results, there is evidence of a lower Average Math Score, lower % Passing Math score,  lower % Passing Reading score and a lower % Overall Passing score.

* How was the school summary affected?

For the school summary table, the only school that shows different results is Thomas High School

Initial Results
![image](https://user-images.githubusercontent.com/26393180/150691376-509a5d61-cb7a-4d3a-82d3-5b2b9683d292.png)

Recalculated Results
![image](https://user-images.githubusercontent.com/26393180/150691394-29a010bd-0266-4f82-96d1-6f06eafc8448.png)

There appears to be a lower calculated average math score and % passing math score. There is also an increase calculated average reading scores. For the overall passing percentage, the percentage has gone down s well. 

* How did replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Initial Results
![image](https://user-images.githubusercontent.com/26393180/150691524-9a207415-4429-4080-9ff0-824d14ed0226.png)

Recalculated Results
![image](https://user-images.githubusercontent.com/26393180/150691534-e213a392-2fb8-4862-be03-82cc761e0abd.png)

After evaluating the top 5 scoring schools, it does appear that Thomas High Schools is still holding the 2nd highest scoring school placement even with the lower % Passing Math scores, % Passing Reading scores and % Overall Passing scores compared to the original analysis.

* How does replacing the ninth-grade scores affect the following:

  * Math and reading scores by grade

Initial Results
![image](https://user-images.githubusercontent.com/26393180/150691603-f2381593-262f-4c29-8f14-158307b68a45.png)

Recalculated Results
![image](https://user-images.githubusercontent.com/26393180/150691624-a013e62b-d754-4b0f-8fd6-521ff5e5148b.png)
After evaluating the math and reading scores by grade, the data shows the only value effected by the adjustment was the 9th grade math and reading scores for Thomas High School. The rest of the data was not impacted

  * Scores by school spending

Initial Results
![image](https://user-images.githubusercontent.com/26393180/150691655-2a081a8a-1e10-4235-b06b-55723b54ccc7.png)

Recalculated Results
![image](https://user-images.githubusercontent.com/26393180/150691666-a59ba026-442e-45bb-be43-612b9fb9667b.png)

The scores by school spending were not impacted by the removal of the 9th grade test scores for Thomas High School

  * Scores by school size

Initial Results
![image](https://user-images.githubusercontent.com/26393180/150691689-3ea00258-7a8b-448d-959b-a4fc6f0cd468.png)


Recalculated Results
![image](https://user-images.githubusercontent.com/26393180/150691697-b5a8b3f8-b384-4b62-92fb-f2a7c55e81b1.png)
The scores by school were not impacted by the removal of the 9th grade test school from Thomas High School

  * Scores by school type

Initial Results
![image](https://user-images.githubusercontent.com/26393180/150691712-abc19e7a-e896-4ff2-aa5f-062a591e1737.png)

Recalculated Results
![image](https://user-images.githubusercontent.com/26393180/150691720-13d7bd59-c4e8-4cd9-bc4e-7da2ba2d708f.png)
The scores by school type were not impacted by the remove of the 9th grade tests scores for Thomas High School.

# Summary

Overall, there were some differences between the initial results and recalculated results
* The district summary results showed lower scores compaired to the initial results. The variables showing a decrease were the average math score, % passing math score, % pssing reading score and the % overall passing.
* The school summary results showed a lower calculated average math score, % passing math score and overall passing percentage. There was also an increase in average reading scores.
* After evaluating the math and reading scores by grade, the data shows the 9th grade math and reading scores for Thomas High Schools were impacted while the rest of the data was unchanged.
* When compairing Thomas High School with the other schools, the DataFrame shows there is a lower % Passing Math scores, lower % Passing Reading scores and a lower % Overall Passing scores compared to the initial results. Even with these changes, Thomas High School still shows to be the second highest scoring school overall. 



