# BitHash Cryptocurrency Exchange Public API (v3)

Public API is used to provide access to the list of used currencies with real-time market data on each.

If you get a "request exceeded" error drop us a message for a private API endpoint.

There are four methods: info, ticker, depth, trades

More info at: https://bithash.info/en/api

# info

Type: GET
Endpoint: /api/info

Parameters: none

Method provides information on active pairs: currency scale (number of digits to the right of the decimal point), minimum price, maximum price, minimum order amount, market status, trading fee.

Example:

https://bithash.info/api/info

# ticker

Type: GET
Endpoint: /api/ticker

Parameters: none or various hyphen-separated currency pairs (example: btc_usd-btc_rub)

Method provides information on active markets for the past 24 hours: maximum price, minimum price, average price, trading volume, trading value, last price, buy price, sell price.

With no parameters passed you get information on all active pairs.

Examples:

https://bithash.info/api/ticker  
https://bithash.info/api/ticker/btc_usd     
https://bithash.info/api/ticker/btc_usd-btc_rub  

# depth

Type: GET
Endpoint: /api/depth

Parameters: none or various hyphen-separated currency pairs (example: btc_usd-btc_rub)

Method provides information on active order books: sell orders (ASK), buy orders (BID).

With no parameters passed you get information on all active pairs.

Examples:

https://bithash.info/api/depth  
https://bithash.info/api/depth/btc_usd  
https://bithash.info/api/depth/btc_usd-btc_rub  

# trades

Type: GET
Endpoint: /api/trades

Parameters: none or various hyphen-separated currency pairs (example: btc_usd-btc_rub)

Method provides information on the last active trades: type, price, amount, trade ID, timestamp.

With no parameters passed you get information on all active pairs.

Examples:

https://bithash.info/api/trades  
https://bithash.info/api/trades/btc_usd  
https://bithash.info/api/trades/btc_usd-btc_rub  
