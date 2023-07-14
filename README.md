# Stock-digging (if trade follows the index of Large order purchase volume)
Since block trading reflects the inflow and outflow of institutional funds, analyzing block trading behavior can explore the relationship between institutional funds and individual stock price movements. This study plans to use Python to conduct statistical analysis on the block trading data of the Shanghai and Shenzhen markets, with a focus on examining individual stock price trends after net block inflows.

The result is NOT WORK WELL when it comes to a daily trade -- t day we buy the stock as the large order comes and day_t+1 we sell it, here is the result. 

Here is the final result:
![(big money png)](https://github.com/shenshenland/stock-digging-/blob/main/big%20money%20png.png)https://github.com/shenshenland/stock-digging-/blob/main/big%20money%20png.png

1. Issues that the huge difference between column change and price change everyday.
   I deal it with using average data:
      here is the way:
   a. using the A =abs(all the data)
   b. using the AVe =average(A)
   c. using every data divided by AVe:every_data/ Ave
   In this way, we get the percentage change
   I did the same when it comes to the trade volumn
 
