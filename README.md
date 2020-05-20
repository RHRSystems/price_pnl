# price_pnl
A command line utility to check your investment prices and PnL.

This is written in Python and uses yahoo_fin and iexfinance libraries to get pricing information.  You must get your own token from IEX and predefine the securities you are interested in the following dictionaries:

dict_names - enter the symbol and type (E for ETF, S for Stock, M for Mutual Fund)
dict_indexes - enter the Indexes you want to follow (symbol and description)
dict_holdings - enter your positions (symbol and quantity)

Here are the options you can use:

With no arguments:
          price_pnl (returns pricing for all predefined Indexes/Stocks/ETF/Mutual Funds, then day PnL


-t (type)

examples:

          price_pnl -t i (returns pricing for your predefined Indexes)
          
          price_pnl -t s (returns pricing for your predefined Stocks/ETFs)
          
          price_pnl -t m (returns limited pricing for your predefined Mutual Funds)
          
          price_pnl -t p (returns day PnL for your predefined positions)



-x (check for one synmbol)

examples:

          price_pnl -x csco (returns pricing for csco then day PnL if you have a position in it)
          
          
