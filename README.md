# Manage-Your-Investment-Portfolio-Part-1
This is a part 1 series of elementary finance analysis using Python

In this Jupyter Notebook file, an example how to keep an overview of your investment
portfolio is provided. The focal point is BTC price performance and return on investment
(ROI), if one would have carried out the following transactions on a Binance crypto exchange: 

*(dd.mm.yy)*
26.04.21 (midnight, £300), 01.06.21 (8pm, £300), 01.01.22 (9pm, £300), 01.06.22 (8pm, £300) → CEST time zone.

## Breakdown of the file:

Cell 1 → (lines are written in Python) Here we connect to the Binance API, which helps us in generating an OHLC (open-high-low-close) DataFrame, starting on 26.04.21 (midnight) and ending on today’s date, i.e. the day when one runs the cell.

Cell 2 → For further calculations, we take “Close” price of BTC and generate a set of four £300 transactions. Since the BTC price data is in USD, the transactions must be converted (exchange rate for that specific day was considered). As with every crypto exchange, fees must be paid and are considered (£5 fee may serve as an illustration). Investment must be overseen and hence profit/loss data is generated. In addition, the following set of data is calculated: the percentage of profit/loss vs the total investment, the percentage of change, i.e. profit/loss for every 2 hours together with the change in USD, BTC price required for the investment to be even and cumulative return of BTC, starting on 26.04.2021.

Cell 3 → Python packages for graphical illustration of data generated in cell 2 are imported.

Cell 4 → General code for graph plotting in Python (Matplotlib). The following graphs are created: BTC price, profit/loss in USD, actual USD owned and pie chart (amount invested vs fees), everything from 26.04.21 onwards.

Cell 5 → As in cell 4, however the additional created graphs are: profit/loss volatility and distribution (every 2 hours), hypothetical BTC price for the investment to be even and pie chart demonstrating the percentage of time being in profit/loss.

Cell 6 → Graphs created are: the percentage of profit/loss for the total investment (a regular plot and a box plot) from 26.04.21 onwards.

Cell 7 → Graphical representation of a BTC cumulative return. 

Cell 8 → Numerical representation for profit/loss in USD via pandas groupby.

Cell 9 → As in cell 8 for USD owned.

## Summary
As of the date of upload, the investment numbers are in red. Such conclusion is not surprising, given the bear market rally in crypto and stock market. While this example shows analysis for BTC, the same approaches are applicable for other cryptocurrencies or stocks.


