# School_District_Analysis
# A Written Report for the School District Analysis 
## Resources:
  - PyCitySchools: represents my first anlysis (including Thomas High School ninth-grade scores.
  - PyCitySchools_Challenge: represents my analysis excluding Thomas High School ninth grade scores to prove academic dishonesty.
  - Resource Folder: Containes all of the csv files I used to determine my analysis and findings. 
  
## 1. Overview of the School District Analysis: Explain the Purpose of the Analysis 
The first analysis I completed *PyCitySchools* was used to help Maria (a chief data scientist for a city school district) analyze data on student funding and students' standardized test scores. To perform my analysis I was given access to every student's math and reading scores as well as various information on the schools they attend. My task was to aggregate the data and showcase the trends in school performance. My analysis helped assist the school board and superintendent in making decisions regarding the school budgets and priorities. My second analysis *PyCitySchools_Challenge* helped Maria and her supervisor provide evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth-graders which appeared to have been altered. I helped Maria prove the extent of the academic dishonesty by replacing the math and reading scores for Thomas High School with "NaNs" while keeping the rest of the data intact. After doing so, I repeated my previous analysis which then helped Maria and I compare the difference to write up a report to describe how these changes affected the overall analysis. 

## 2. Results
### How is the School Summary Affected:
The disrict summary BEFORE replacing the Thomas High School ninth-grade class with "NaNs" is shown in the following table below: 
<img width="1087" alt="Screen Shot 2022-06-02 at 12 39 41 PM" src="https://user-images.githubusercontent.com/104043438/171702646-6c1da631-c3da-4b05-8a27-21791b378a87.png">
As you can see the overall passing percentage was 65%. 

The district summary AFTER replacing the Thomas High School ninth-grade class with "NaNs" is shown in the following table below: 
<img width="1083" alt="Screen Shot 2022-06-02 at 12 41 57 PM" src="https://user-images.githubusercontent.com/104043438/171703023-69f69d11-5f52-4353-a013-066bd80de467.png">
As you can see the overall passing percentage decreased to 64.9%, though it's a small change, I was curious to see how many 9th grade students there were at Thomas High School. Therefore, using the "COUNTSIS" function in excel I determined the exact amount of students in the ninth-grade class.
##### =COUNTSIF(D:D,"Thomas High School", E:E, "9th")=461 total ninth graders attending Thomas High School. 
##### Of the 15 schools their was a total of 39,170 students divided by 461 ninth graders at THS = 0.1176921 * 100 = 1.1769211 (%1.18). Thus, the ninth-grade students attending Thomas High School only made up %1.18 of the total students used in my data findings. So, even though the district summary only experienced a %0.1 decrease in overall passing students, that is a big difference when you consider how little the ninth-grade class was compared to the overall population of students. 

### How is the District Summary Affected:
No, after reveiwing my previous explanation it's important to note that out of the 15 schools I used in my analysis, their are two subcategories: district and charter schools. Since Thomas High School (THS) is a charter school the overall district summary wasn't affected. As you can see from the table below, charter schools, however, expeirenced a 36% overall higher passing compared to the district schools.

<img width="825" alt="Screen Shot 2022-06-02 at 1 42 38 PM" src="https://user-images.githubusercontent.com/104043438/171724971-efca5a0c-c19c-443f-bb76-cac6621ddf76.png">

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools: 
In my first analysis *PyCitySchools* you can see that when the analysis included (THS) ninth-grade math students the school's average passing math percentage was %93.87. View the table below for evidence. 
<img width="1071" alt="Screen Shot 2022-06-02 at 1 59 32 PM" src="https://user-images.githubusercontent.com/104043438/171728211-a4e0ce0e-467e-4625-8c83-3cfdb708cbb8.png">
In my second analysis when I replaced (THS) ninth-grade math class with "NaNs", the new average passing math percentage decreased to %66.91. View the table below for evidence. 
<img width="1069" alt="Screen Shot 2022-06-02 at 2 00 02 PM" src="https://user-images.githubusercontent.com/104043438/171728394-5a6c94db-e7d5-4e6a-8662-8de65c4f67e0.png">
It can now be said that due to (THS) changing their ninth-grade math scores, the average score for students passing math increased but in reality, it should've decreased because those scores weren't an accurate representation of the students' true grades. 
