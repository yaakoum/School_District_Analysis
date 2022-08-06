# School District Analysis using PyCitySchools

## Overview of the School District Analysis
This project revolves around helping Maria analyze data on student funding and students' standardized tests scores. The challenge is to showcase trends in school performance in order to make decision on school budgets. 

## School District Analysis Results

### How is the district summary affected?
- The district summary barely changes as removing the 9th graders from one school does not account for a lot from the total number of students. The original district summary results are as follows:

![District Summary Original](https://github.com/ayaakoub/School_District_Analysis/blob/main/Resources/District_Summary_Original.PNG)

And the adjusted are as shown:

![District Summary Adjust](https://github.com/ayaakoub/School_District_Analysis/blob/main/Resources/District_Summary_Adjusted.PNG)

- It can be seen that there are 39,170 students in total from all districts, a count of the ninth graders at Thomas High yields 461 students. The grades from those 461 students has an impact of less than a 1% (0.1% to be exact on math and reading averages).

### How is the school summary affected?
- The first image below shows the school's averages with the ninth graders included, and the second is with the ninth graders math and reading scores switch to NaN (excluded from the average). The average remains very similar and that is due to the fact that the grades were probably close to the average and therefore have no effect. 
Original:
![Original Per Summary](https://github.com/ayaakoub/School_District_Analysis/blob/main/Resources/Per_Summary_Original.PNG)
Adjusted:
![Adjusted Per Summary](https://github.com/ayaakoub/School_District_Analysis/blob/main/Resources/Per_Summary_Adjusted.PNG)

- However, the average scores and percentages were mostly effected when a new average was taken by eliminating the 9th grader student count. Since just converting the student grades to NaN did not reduce the total number of student count. When the new count was used the average was adjusted significantly (increased) as shown below:

![Adjusted District Summary](https://github.com/ayaakoub/School_District_Analysis/blob/main/Resources/THS_updated_summary_dataframe.png)

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

- As seen in the previous images, both times Thomas High came in second when the data was organized by the '% Overall Passing'. Replacing the ninth graders math and reading scores to NaN did not skew the overall results as much. 

- However, when a new average was calculated using the new averages which excludes the student count from the 9th grade Thomas High School went down significantly.

### Replacing the ninth-grade scores affect the following:
- Math and reading scores by grade
  The math and reading score for the school remained very similar as shown above. All the 9th grade scores were NaN for Thomas High School.
- Scores by school spending
  The spending buckets had to be adjusted to be more even amongest the schools. The ranges were different and therefore the averages were different. 
- Scores by school size
  The scores by school size did not change as much since the overall number of students in each bucket is large and the effect of the change in Thomas High School by itself did not have a huge impact.
- Scores by school type
  Similar to above each bucket (Charter and District) are large and contain a lot of other schools and so the change from Thomas High does not have much of an impact both results can be seen below, original and adjusted, respecitvely. 
Original:
![Original Type Summary](https://github.com/ayaakoub/School_District_Analysis/blob/main/Resources/Type_Summary_Original.PNG)
Adjusted:
![Adjusted Type Summary](https://github.com/ayaakoub/School_District_Analysis/blob/main/Resources/Type_Summary_Adjusted.PNG)
## School District Analysis Summary

There are many differences that occured when the ninth graders scores were removed: 

- The overall passing rate for Thomas High School can be seen above as changed dramatically, increased (65% to 91%), when 9th grader scores and student count were excluded. 
- The above increase caused the school to drastically change its rating in the district. 
- A slight shift was across the district and across the 9th grade average. 
- All Thomas High School Ninth graders score now are shown as NaN. 
Footer
© 2022 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
