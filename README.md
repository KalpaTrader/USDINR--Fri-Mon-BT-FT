# USDINR--Fri-Mon-BT-FT
Strategy backtest of Friday Long , Monday Exit for USDINR futures

The strategy seeks seasonality for day of week in USDINR futures. It is seen that Monday is usually associated with gains in the pair i.e rupee becomes weaker. 

This can be partially due to the weekend effect for the Dollar Index -safe haven /risk off hedge flows.

Another reason could be due to the phenomenon discussed in https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3138756 as Indian currency markets close at 5 P.M. indian time, right about the time when the US markets open.

Since the expiry of the pair is on Friday, there are large jumps in data. To counter this, price of the contract one day before expiry is taken and the new contract price is taken for the expiry day. Then a backward adjusted average of the prices is taken to create a time series.

The results are promising with the effect prominent equally  in the in-sample - 2010-2017 and out-of-sample 2018-2022 data.

Special thanks to @AnkitQuant (twitter) who's monty carlo code I have shamelessly copied as it was neat. https://medium.com/@ankit_quant/when-to-stop-trading-a-strategy-28d104bb20b6
