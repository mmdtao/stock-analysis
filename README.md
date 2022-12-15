# Steve's All Stocks Analysis

## Overview of Project
Steve, who has just graduated with his finanace degree, is looking to analyze green energy stocks for his parents. He wants to diversify his parents' portfolio outside of silicon wafers.

### Purpose
Specifically, Steve would like a macros that can analyze all the green stocks, currently and for the future, so that he can help his parents make the profitable investments in green energy. The data contains daily starting and ending prices for each ticker and the day's corresponding volume. This macro will be able to analyze the stocks provided by year (2017 or 2018) and compiles each ticker's "Total Daily Volume" and "Return" making it simpler to visually see the profitability of each stock.

## Analysis + Results
By using loops to run through the data, ticker volumes can be stored in an array for each specific stock as shown in step "2a" below. The macro then runs through each row aggregating the ticker volumes, then starting prices, and lastly ending prices. Each time a loop is completed, the tickerIndex is increased so that the next row of data can be iterated. 

<img width="786" alt="Loop through spreadsheet" src="https://user-images.githubusercontent.com/114324871/207759812-848b932d-e68a-4ac1-964b-936a8802be95.png">

Next, the macro outputs each ticker and its corresponding values of "Total Daily Volume" and "Return" into a table format. The return is calculated by taking the tickerEndingPrices and dividing it by tickerStartPrices to create a percentage useful to understand whether the stock is increasing or decreasing in value.

<img width="614" alt="Loop through arrays" src="https://user-images.githubusercontent.com/114324871/207759841-bdd446d9-3f32-4154-b4e0-5956bf36c516.png">

### Results
Comparing the stock returns from 2017 and 2018, only two stocks (ENPH and RUN) show a yearly increase in return. While Steve's parents had seen a lot of growth in their green energy stocks in 2017 highlighted by the green cells, 2018 saw a decline in return for nine of the previously profitable stocks highlighted by the switch in cell color from green to red. So based on the 2018 returns, I would suggest they may see more sustained growth in the ENPH and RUN tickers.

<img width="345" alt="AllStocksAnalysis2017" src="https://user-images.githubusercontent.com/114324871/207778702-0897294f-b8fc-4654-9dae-917d31986c46.png">

<img width="263" alt="VBA_Challenge_2017" src="https://user-images.githubusercontent.com/114324871/207759743-6859d936-deb0-4c6a-a833-f6719ce7df53.png">

<img width="341" alt="AllStocksAnalysis2018" src="https://user-images.githubusercontent.com/114324871/207778725-a42c019f-237e-4742-bcf9-2c709b75a99d.png">

<img width="263" alt="VBA_Challenge_2018" src="https://user-images.githubusercontent.com/114324871/207759745-ddbd8476-50e2-4327-92c9-828183748a3f.png">

## Summary

### Advantages and Disadvantages of Refactoring Code
Refactoring code simplifies and makes code more readable to any future user. Future users would be able to more quickly debug and maintain software saving everyone time and resources. Highlighted in this challenge we see that by refactoring the code from the module, we lessen the run time of our macros. Refactoring also has the ability to introduce new bugs and errors. If a team were working on refactoring, coordination of improvements to the code could become convoluted as copies drift from the original code.

In this challenge, refactoring reduced the run time by around a second signifying the efficiency created by the refactored loops. The disadvantage of refactoring this code is the amount of variables increased, adding to the complexity of the code in a way that future changes could easily produce errors rendering the overall code useless.




