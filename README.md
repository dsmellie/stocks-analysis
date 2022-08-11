# Analysis of Green Stock Returns Refactored

## Overview of Project
This project analyzed the returns of a number of green stocks in 2017 and 2018.

## Purpose
The purpose of this analysis is to help Steve's parents invest in green stocks. 

## Analysis and Challenges
To analyze these returns I compared the starting and ending prices of stock over the year and determined the percentage change. One challenge was refactoring the code so that it could be used in the future.  The main challenge I encountered in refactoring the code was ensuring the data was properly output and making sure to use the correct index for the arrays I created. 

## Results
The first result of note is that only two stocks had a positive performance in 2018, ENPH and RUN as shown below.

[VBA_Challenge_2018](https://user-images.githubusercontent.com/109701875/184050036-8d81e0c9-6a4f-4765-b1ba-1779e7d36880.png)

As these stocks also performed positively in 2017, they may represent good investments. However, several stocks in 2017 seriously outperformed RUN. DQ, ENPH, FSLR, and SEDG all had returns over 100% for 2017 while RUN only had a 5.5% return as seen below. 

![VBA_Challenge_2017](https://user-images.githubusercontent.com/109701875/184050342-81c5b157-b40d-4509-957f-e9b64c95e9da.png)

Because of the difference in years, I calculated the two-year returns shown below. I calculated the returns by doing = (1+M4) * (1+N4) - 1 and so on. Or to put it generically, (1+2017return) * (1+2018return) - 1. 

![VBA_2year_Returns](https://user-images.githubusercontent.com/109701875/184050682-e26284d7-19a5-43da-aeb4-3f18524afea3.png)

Based on these two year results, ENPH, RUN, and SEDG are the best investments. 

###Limitations

There are several limitations on this data. First, it only covers two years worth of returns. As seen in the returns themselves, performance can vary drastically year over year and so more years of data would help the analysis, especially more recent years. Second, although the daily volume and return are usual information they are far from the only information to consider before buying a stock. Some other information that would be helpful to have access to include accounting information (gross/net revenues, EBITDA, etc.), any upcoming or recent mergers, and the price-to-earnings ratio of the stock are all factors commonly considered in stock purchases that we do not have access to. 

##Summary

###Advantages and Disadvantages of Refactoring Code

The choice to refactor code has clear advantages and disadvantages. The biggest advantage of refactoring code is that it helps futureproof the code such that changes down the line do not render the code non-operational. Refactoring can help make the code more readable and easier to change in the future. It can also serve to save time in the future by preventing the need to redo work. Refactoring code can also improve the runtimes and efficiency of the code refactored. 

The biggest disadvantage of refactoring code is that it takes time and that time may not be recovered if the code is not changed or reused. Refactoring also risks breaking the code and being unable to successfully refactor the code

###Advantages and Disadvantages of AllStocksAnalysisRefactored

