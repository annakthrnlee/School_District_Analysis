# School_District_Analysis
# A Written Report for the School District Analysis 
## Resources:
  - PyCitySchools: represents my first anlysis (including Thomas High School ninth-grade scores.
  - PyCitySchools_Challenge: represents my analysis excluding Thomas High School ninth grade scores to prove academic dishonesty.
  - Resource Folder: Containes all of the csv files I used to determine my analysis and findings. 
  
## 1. Overview of the School District Analysis: Explain the Purpose of the Analysis 
The first analysis I completed *PyCitySchools* was used to help Maria (a chief data scientist for a city school district) analyze data on student funding and students' standardized test scores. To perform my analysis I was given access to every student's math and reading scores as well as various information on the schools they attend. My task was to aggregate the data and showcase the trends in school performance. My analysis helped assist the school board and superintendent in making decisions regarding the school budgets and priorities. My second analysis *PyCitySchools_Challenge* helped Maria and her supervisor provide evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth-graders which appeared to have been altered. I helped Maria prove the extent of the academic dishonesty by replacing the math and reading scores for Thomas High School with "NaNs" while keeping the rest of the data intact. After doing so, I repeated my previous analysis which then helped Maria and I compare the difference to write up a report to describe how these changes affected the overall analysis. 

## 2. Results
### How is the District Summary Affected:
The disrict summary BEFORE replacing the Thomas High School ninth-grade class with "NaNs" is shown in the following table below: 
<img width="1087" alt="Screen Shot 2022-06-02 at 12 39 41 PM" src="https://user-images.githubusercontent.com/104043438/171702646-6c1da631-c3da-4b05-8a27-21791b378a87.png">
As you can see the overall passing percentage was 65%. 

The district summary AFTER replacing the Thomas High School ninth-grade class with "NaNs" is shown in the following table below: 
<img width="1083" alt="Screen Shot 2022-06-02 at 12 41 57 PM" src="https://user-images.githubusercontent.com/104043438/171703023-69f69d11-5f52-4353-a013-066bd80de467.png">
As you can see the overall passing percentage decreased to 64.9%, though it's a small change, I was curious to see how many 9th grade students there were at Thomas High School. Therefore, using the "COUNTSIS" function in excel I determined the exact amount of students in the ninth-grade class.
##### =COUNTSIF(D:D,"Thomas High School", E:E, "9th")=461 total ninth graders attending Thomas High School. 
##### Of the 15 schools their was a total of 39,170 students divided by 461 ninth graders at THS = 0.1176921 * 100 = 1.1769211 (%1.18). Thus, the ninth-grade students attending Thomas High School only made up %1.18 of the total students used in my data findings. So, even though the district summary only experienced a %0.1 decrease in overall passing students, that is a big difference when you consider how little the ninth-grade class was compared to the overall population of students. 

### How is the School Summary Affected:
