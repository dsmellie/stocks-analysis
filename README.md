# Analysis of Green Stock Returns Refactored

## Overview of Project
This project analyzed the returns of a number of green stocks in 2017 and 2018.

## Purpose
The purpose of this analysis is to help Steve's parents invest in green stocks. 

## Analysis and Challenges
To analyze these returns I compared the starting and ending prices of stock over the year and determined the percentage change. One challenge was refactoring the code so that it could be used in the future.  The main challenge I encountered in refactoring the code was ensuring the data was properly output and making sure to use the correct index for the arrays I created. 

### Analysis of Outcomes Based on Launch Date
To analyze the outcomes based on launch date, I used a PivotTable. I filtered the PivotTable based on years and parent category. I put the outcomes into columns, count of outcomes in values, and date created in rows as shown in the screenshot below.
![Pivottable](https://user-images.githubusercontent.com/109701875/182739203-1bb582bf-8860-4317-ace2-59581b0f1a7b.PNG)!

 

I then made a line graph to show how each month compared.
 ![image](https://user-images.githubusercontent.com/109701875/182731431-badfe07c-aa4d-436b-a77c-abc4deca1364.png)

### Analysis of Outcomes Based on Goals
To analyze the outcome based on goals, I used COUNTIFS to determine the number of successes, failures, and cancels for each category. For example, I used the code COUNTIFS(Kickstarter!D:D, "<1000",  Kickstarter!F:F, "successful") to determine the number of successful campaigns that aimed to raise under $1000. After calculating the number of successes, failures, and cancels I used SUM to determine the total number of projects in each category. For example, I used the code =SUM(B2:D2) to determine the number of successful campaigns that aimed to raise under $1000. Then, I calculated the percentage of successes, failures, and cancels by dividing each by the total number of projects.  For example, I used the code =B2/E2 in a percentage box to determine 75.81% of all finished projects that try to raise under $1000 are successful. Then I made the line graph below.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/109701875/184043368-9c91b4e3-f0d2-4456-991b-455faf3df9ff.png)


### Challenges and Difficulties Encountered
The sole difficulty I had was getting my dataset for Outcomes based on!
 Goal to match the expected output. I quickly found the error I made was that rather than analyzing based on the goal data, I had instead used the amount pledged data. By fixing this mistake, I was able to output the expected graph. 
## Results
The first result of note is that only two stocks had a positive performance in 2018, ENPH and RUN as shown below.

[VBA_Challenge_2018](https://user-images.githubusercontent.com/109701875/184050036-8d81e0c9-6a4f-4765-b1ba-1779e7d36880.png)

As these stocks also performed positively in 2017, they may represent good investments. However, several stocks in 2017 seriously outperformed RUN. DQ, ENPH, FSLR, and SEDG all had returns over 100% for 2017 while RUN only had a 5.5% return as seen below. 

![VBA_Challenge_2017](https://user-images.githubusercontent.com/109701875/184050342-81c5b157-b40d-4509-957f-e9b64c95e9da.png)

