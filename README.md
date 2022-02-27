```diff
- API v3 is no longer maintained and will be depreciated soon 
```

An updated list of BitHash API's:

https://support.bithash.net/hc/en-us/sections/360004615352-API

# BitHash Cryptocurrency Exchange Public API (v3)

Public API is used to provide access to the list of used currencies with real-time market data on each.

If you get a "request exceeded" error drop us a message for a private API endpoint.

There are four methods: info, ticker, depth, trades

More info at:  
  
https://www.bithash.net/en/api 

# info

Type: GET
Endpoint: /api/info

Parameters: none

Method provides information on active pairs: currency scale (number of digits to the right of the decimal point), minimum price, maximum price, minimum order amount, market status, trading fee.

Example:

https://www.bithash.net/api/info

# ticker

Type: GET
Endpoint: /api/ticker

Parameters: none or various hyphen-separated currency pairs (example: btc_usd-btc_rub)

Method provides information on active markets for the past 24 hours: maximum price, minimum price, average price, trading value, trading volume, last price, buy price, sell price.

With no parameters passed you get information on all active pairs.

Examples:

https://www.bithash.net/api/ticker  
https://www.bithash.net/api/ticker/btc_usd     
https://www.bithash.net/api/ticker/btc_usd-btc_rub  

Note:

vol_cur = Trading Volume
vol = Trading Value

vol_cur -> BTC/USD <- vol

# depth

Type: GET
Endpoint: /api/depth

Parameters: none or various hyphen-separated currency pairs (example: btc_usd-btc_rub)

Method provides information on active order books: sell orders (ASK), buy orders (BID).

With no parameters passed you get information on all active pairs.

Examples:

https://www.bithash.net/api/depth  
https://www.bithash.net/api/depth/btc_usd  
https://www.bithash.net/api/depth/btc_usd-btc_rub  

# trades

Type: GET
Endpoint: /api/trades

Parameters: none or various hyphen-separated currency pairs (example: btc_usd-btc_rub)

Method provides information on the last active trades: type, price, amount, trade ID, timestamp.

With no parameters passed you get information on all active pairs.

Examples:

https://www.bithash.net/api/trades  
https://www.bithash.net/api/trades/btc_usd  
https://www.bithash.net/api/trades/btc_usd-btc_rub  


---

# About BitHash

BitHash Cryptocurrency Exchange was established in 2016 in Singapore with more than 100 pairs available for trading cryptocurrency - Bitcoin (BTC), Ethereum (ETH), Litecoin (LTC), Bitcoin Cash (BCH), Ethereum Classic (ETC), Dash (DASH), EOS (EOS), TON Coin (TON), Monero (XMR), Ripple (XRP), Zcash (ZEC).

BitHash Exchange is operated by PHOENIX TRADING SOLUTIONS LTD, a licensed company incorporated under the International Business Companies Act of 2016 of the Republic of Seychelles with company number 214028.

Global Gateway 8, Rue de la Perle, Providence, Mahé, Seychelles
PHOENIX TRADING SOLUTIONS LTD.
IBC NO 214028

https://www.bithash.net/
