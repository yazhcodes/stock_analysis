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
Before getting to refactor my code as per course instructions, I tried a different variation of the analysis logic. Instead of a Nested For loop as mentioned in the course, I tried to use accomplish the task using just one For Loop. My idea was to optimize the code by cutting down the number of times the loop executed. The Nested FOR loop looped through the data set 36144 (12 * 3013) and my method looped through the data only 3012 times. Surprisingly, there was not much of a difference in terms of execution time. 

**Refactoring using Arrays**
So I went on to refactor my code based on the logic used in the course, which was using one FOR loop and several arrays to store the calculated values. It was interesting to see that using multiple arrays reduced my run time significantly. I realized that switching between worksheets, going back and forth multiple times to analyze and output the calculated values had caused my analysis to slow down a lot. Instead staying on one sheet for the entire analysis, storing the calculated values in arrays and then populating the outputs on a different sheet in the very end cut down my runtime by half. The stats of my findings can be found below.

Execution Time 

## SUMMARY

What are the advantages or disadvantages of refactoring code?

How do these pros and cons apply to refactoring the original VBA script?
