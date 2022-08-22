# Stock-analysis

## Overview of Project
The goal of this project was to write a script in VBA to analyze specific years of stock trends as quick as possible. We were asked by Steve to analyze two years worth of stock information and determine the best stocks to invest in. We completed this task in two different ways, one being faster than the other.

## Results
From our results we can see that 2017 was a much better year for the majority of stocks. We can also see that ENPH will be the best stock to invest in long term. We can tell this because it had both strong positive returns both in 2017 and 2018. 
### Original Code
In our original code, it wasen't the best way to get the job done but it did go through all the tickers and determine the returns for each one. We can see that using a nested for loop with multiple if-then statements will get the job done but it did take a little bit of time to process (see examples below)

![image](https://user-images.githubusercontent.com/109539205/185936526-8b8b08bc-9b18-41de-b13c-cc6b5dec4f3b.png)
![Green_stocks_2017](https://user-images.githubusercontent.com/109539205/185936608-2850fde0-455c-456f-af8e-93394a1ccfa6.png)
![Green_stocks_2018](https://user-images.githubusercontent.com/109539205/185936630-98fde30c-0304-422c-8ba6-c9244994ea9b.png)
this code took about .4 seconds to run and complete, but we can definitely make this faster, which we did. 

### Refactored code
In our refactored code, we took what we already had and made it a bit cleaner so that it would run faster. This would be helpful in situations where we are analyzing multiple years and a lot more data. In our refactoring we used nested for loops as well as arrays to store the data to be accessed a little easier. By looping through these arrays while also looking for the ticker name and index, We can completly cut the last step of the original code which looks through the rows for the appropriate information. After refactoring our code we were able to cut the run time down to .1 second and sometimes even lower. Below is images of the refactored code being ran.![VBA_Challenge_2017](https://user-images.githubusercontent.com/109539205/185938795-8f2bcdeb-f600-443a-a0c1-3c8ead243813.png)
![VBA_Challenge_2018](https://user-images.githubusercontent.com/109539205/185938812-70a02f87-a6da-429d-9fed-b792d305d474.png)

##Summary
There is clearly an advantage to refactoring code. Sometimes there is multiple ways to solve a problem but one can be better than the other. It could save everyone a lot of time when working with huge datasets. In this case, refactoring this stock analysis code saved us 4 times the amount of time. While that may not be a huge difference when we are talking both being less than a second, the code was better organized and could be read a little easier by another person on a team.
