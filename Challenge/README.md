# STOCK ANALYSIS

## OVERVIEW OF PROJECT

This project is about analyzing Green energy stock data of a dozen tickers to identify the ones that would be best to invest in, based on their Total Daily Volume and Returns in the past couple of years.

## RESULTS

Using images and examples of your code, compare the stock performance between 2017 and 2018, as well as the execution times of the original script and the refactored script

### Stock Performance in 2017 vs 2018

Upon comparing and visualizing the stock returns of various tickers over 2017 and 2018, it is quite evident that Green energy has suffered a significant loss in 2018, with the exception of ***Sunrun Inc***, a Solar Company that has seen an increase in return of over 78% in two years. It is undoubtedly the best green stock to invest at this point of time.

<p align="center"><img src="https://github.com/yazhcodes/stock_analysis/blob/main/Challenge/Resources/2017vs2018.png"></img></p>

### A comparison of Execution Time

**Nested FOR Loop vs FOR Loop**

Before getting to refactor my code as per course instructions, I tried a different variation of the analysis logic. Instead of a Nested FOR loop as mentioned in the course, I tried to accomplish the task using just one FOR Loop. My idea was to optimize the code by cutting down the number of times the loop executed through the dataset. The Nested FOR loop looped through the data set 36144 (12 * 3013) times and my approach using just one FOR Loop looped through the data only 3012 times. This cut down the execution time by 0.2 seconds. 

**Refactoring using Arrays**

Then I went on to refactor my code based on the logic used in the course, which was using one FOR loop and several arrays to store the calculated values. It was interesting to see that using multiple arrays reduced my run time significantly. I realized that switching between worksheets, going back and forth multiple times to analyze each ticker and output the calculated values before moving on to the next ticker, had caused my analysis to slow down a lot. Instead staying on one sheet for the entire analysis, storing the calculated values in arrays for all tickers and finally populating the outputs on a different sheet in the very end cut down my runtime by another 0.2 seconds. The stats of my findings are below.

<p align="center"><img src="https://github.com/yazhcodes/stock_analysis/blob/main/Challenge/Resources/Execution_Time.png" width="350"></img></p>

***Execution Time of Final Refactored Code (2017)***

<p align="center"><img src="https://github.com/yazhcodes/stock_analysis/blob/main/Challenge/Resources/VBA_Challenge_2017.png" width="800"></img></p>

***Execution Time of Final Refactored Code (2018)***

<p align="center"><img src="https://github.com/yazhcodes/stock_analysis/blob/main/Challenge/Resources/VBA_Challenge_2018.png" width="800"></img></p>

## SUMMARY

The ADVANTAGES of refactoring according to ***Martin Fowler (Father of Code Smell)*** are stated in the following:

1. **Improves the Design** of Software
2. Makes Software **Easier to Understand**
3. Helps Finding **Bugs**
4. Helps Programming **Faster**

The DISADVANTAGES of refactoring code are,

1. **Time Consuming:** You may have no idea how much time it may take to complete the process. It may also land you into a situation where you have no idea where to go.
2. **Chance of Mistakes:** In case if it went wrong, you will have to waste much more time in solving the problem and there are probable chances that it may go wrong due to complexity of the code.

How do these PROS and CONS apply to refactoring the original VBA script?
  
  The refactored code looks more **organized and professional**, and makes it **easier** for me to pick up where I left off when I take breaks in between. But it is **hard work** if you are not a fan of perfection. Because at this point you have already accomplished the task you were meant to do and every additional minute spent on refactoring code can be considered a waste of **time** especially if you are due to complete the next task.

***References:***
* https://stackoverflow.com/questions/43983284/what-are-the-advantages-and-disadvantages-of-refactoring-code-smell-in-software
* https://anarsolutions.com/code-refactoring-concept-analysis/#:~:text=Maintainability%3A%20After%20refactoring%2C%20the%20code,no%20idea%20where%20to%20go.
