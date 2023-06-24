# BadAssStockPickerAI
A Python file to predict stock prices. Please bear with me it works, but I wouldn't recommend using it to invest yet.

I have been teaching myself both to invest and to program AI. Unfortunately, when I took on this new hobby I knew nothing of programming or AI. I have been
teaching myself Python and have become somewhat competent at some of the necessary libraries--Tensorflow, Pandas, etc.

A lot of this was created through trial and error or by searching on the internet for answers.

As a result:

1)  My commenting might be a bit all over the place and only marginally helpful.
2)  Some vestigial code may be commented out but still in the program.
3)  There may be quite a few areas where something was done in a considerably more complicated manner than necessary, because I was too ignorant to realize a simpler path existed.
4)  A lot of what I did may be head-scratchingly stupid or outside of normal coding practice. Did I mention I am teaching myself?

This program is the result of quite a bit of tinkering. It is the result of several classes on Coursera and Udemy.

One issue I recognize is that the picks tend to be strictly oppositional. A stock will be picked to go up only because it has previously gone down. Anybody who understands
trends would recognize that's not really how stocks work. Another issue is that it chooses a direction and an endpoint, but then acts as if stocks move in a straight line. 
Only problem is that they don't.

Here is a quick overview:

1) The program accesses a .xlsx file that contains holdings from ishares funds. These are accessed only to get a list of tickers and sectors.
2) The program gets data both from yfinance and Alpha Vantage. That, and some variables to pause the program and whatnot, are to overcome usage restrictions.
3) It puts the tickers into a stew which creates randomly divided dataframes of length timeframe, during the specified period (all variables that can be adjusted).
4) The program adds in a number of sector indexes to help with prediction, and some economic data.
5) The final prediction is to be the stock price "future offset" days away (another variable that can be adjusted). I have tried a number of architectures. Mostly RNNs.
6) To be real fancy, the data is saved in an excel spreadsheet. I don't know why, as I never look at the spreadsheets.

I would be really excited to have other people take a crack at the code. Only condition is that you loop me in to what you are doing, so we can get rich together.

