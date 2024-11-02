java c
BUSFIN 1356: FINTECH, Fall 2024 
Assignment 4 
Due: Monday, November 4, 2024 
Coding the Algo – Automated order entry and exit
Most trading is automated, that is, it is driven by algorithms or algos in short. HFT firms use specialized algos calibrated to run faster than others so as to generate arbitrage profits. Buy-side traders, or money managers, use algos to combat HFT centers. All investment banks have been using algos since 1980s. In this exercise, you are going to build an algorithm using the Trading Technologies’ Algo Design Lab (ADL) platform. and report your outcome.
A bracket order is a set of three orders that include the entry order, a take-profit order (limit), and a stop-loss order. It is “bracketed” around a trade, managing both the entry and exit simultaneously. It is primarily used to fully automate trade execution, including both profit-taking and risk management. Once the entry order is filled, the two exit orders (profit and stop-loss) remain active. When one of the exit orders is triggered, the other is automatically canceled. 
Example: 
1.   You place an entry order to buy at $100.
2.   You simultaneously place a take-profit order at $110 and a stop-loss order at $95.
3.   Once the stock is bought at $100, the bracket order ensures that you exit the trade either at $110 (profit) or $95 (loss).
Benefits of a bracket order include:
•    Provides complete trade automation (entry and exit).
•    Protects both profit and limits losses.
•    Useful for day traders who want to manage positions without constant monitoring.
A bracket order’s main drawback is its complexity, where it requires more setup compared to simple order types. That is why analgo must be used to execute this type of order. Also, a basic bracket order offers no flexibility if market conditions change quickly, as both profit and stop-loss targets are predefined. So one must consider improving a bracket order to take into account such changes overtime so it can be fully automated without such concern.
You will use Trading Technologies’ Algo Design Lab to build a bracket algo and test in on your Trading Technologies Account.  Use Google Chrome as your browser.  Other browsers may not work or provide partial functionality; TT has been built to work on Chrome.
First, login to your TT account and create a workspace to conduct your testing and observe your trades.  Click on the workspace you create to launch it and add the “MD Trade代 写BUSFIN 1356: FINTECH, Fall 2024 Assignment 4Prolog
代做程序编程语言r” (use the “ES Dec 24” contract as the instrument), the “Positions,” and the “Fills” widgets to your trading bench. 
Second, while your workspace is open and observable on one screen, click on the “ADL” icon to launch the Algo Design Lab.  You may follow the steps discussed at the ITG Futures siteto build your algo. If this site is no longer functional, usethis static versioninstead.  This site shows a static buy order (no slicing and dicing via iceberg) and does not include the stop loss option for  the exit trade.
If you follow the ITG site, the formulas for the “Value Accumulator” measuring fill quantity is {fillQuantity} and total cost (VAR) is {fillPrice} * {fillQuantity} respectively.  Note how you can use these values to calculate average price of your fills. This is especially useful if you are using an iceberg order to conduct the fills as each piece of the iceberg may be filled at a different price point.
For the logic that drives the exit trades, you may use thisdepiction(also available in the appendix.)
Feel free to build your bracket algo using your own logic without help from the ITG site.
Questions - Take notes during the simulation so you can answer these questions.
1.   Export your algo as a json file on ADL and upload to Canvas.
2.   What parameters (+/- tick size) did you use for your exit orders, namely the limit sell and the stop loss.
3.   Record your closing position, profit or loss.  Provide screenshots to support claims.
4.   Calibrate (via trial and error) your trading parameters and report your profit outcomes for each choice of their values.
5.   Discuss how you can improve your results.  What additional information and code might improve your results?
Bonus Question: Start your exercise by downloading and importingthis VWAP algoprior to building your bracket order and use the VWAP block to make your bracket algo more intelligent. Note the time window variable is measured in milliseconds.
P.S. I provide the following resources foralgo trading should you choose to pursue learning more about automated trading and writing more sophisticated algorithms.
Algo Blocks 
Short ADL Course 
ADL Training Video 
TT ADL Resources 
Finally, for more detailed learning, I recommend the following book written by a colleague, Joel Rubano:
Trader Construction Kit, 2nd Ed. 
Please do not hesitate to contact if you have any questions.






         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
