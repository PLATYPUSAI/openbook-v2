frustrated with the difficulty of running openbook-v2 on Linux Mint I documented the build here. This is likely not complete, but it will help. May the source be with you.
# openbook-v2 settings
openbook-v2 is designed to create an orderbook for liquidity pairing on raydium, jupiter and other Solana DEX a working version of this code is available at <a href="https://openbookdex.space">openbookdex.space</a><br />

Quote Mint: The token you wish to pair with your token as contract address verify on solscan.io yourself

SOL: So11111111111111111111111111111111111111112
USDC: EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v
USDT: Es9vMFrzaCERmJfrF4H2FYD4KCoNkY11McCe8BenwNYB

caveat:
The minimum order size should not exceed the base token’s decimals.
The price tick size should not exceed the quote token’s decimals.
The sum of ‘Minimum order size’ + ‘Price Tick’ should not exceed the quote token decimals.

example settings for min order and min price as variables:

Min. Order Size: Minimum order quantity for the order book.
Example: Set to 0 -> Can place an order for 1 unit.
Example: Set to 1 -> Can place an order for 0.1 unit
Example: Set to 2 -> Can place an order for 0.01 unit
Example: Set to 3 -> Can place an order for 0.001 unit
Example: Set to 4 -> Can place an order for 0.0001 unit
Example: Set to 5 -> Can place an order for 0.00001 unit
Example: Set to 6 -> Can place an order for 0.000001 unit e.g. USDC
Example: Set to 7 -> Can place an order for 0.0000001 unit
Example: Set to 8 -> Can place an order for 0.00000001 unit
Example: Set to 9 -> Can place an order for 0.000000001 unit e.g. Bitcoin

Price Ticker: Number of decimal places for price display.
Example: Set to 0 -> The token price is display as 1 / Solana
Example: Set to 2 -> The token price is displayed with 2 decimal places, like 0.12
Example: Set to 3 -> The token price is displayed with 3 decimal places, like 0.123
Example: Set to 4 -> The token price is displayed with 4 decimal places, like 0.1234
Example: Set to 5 -> The token price is displayed with 5 decimal places, like 0.12345
Example: Set to 9 -> The token price is displayed with 9 decimal places, like 0.123456789


reminder
The minimum order size cannot exceed the base token’s decimals. For instance cannot buy .000000001 of .0001 as the orderbook is measuring to a setting of 4

The price tick size should not exceed the quote token’s decimals. While it is nice to read micro amounts of a token, setting the price tick to 1 is easy for buyers to understand.

The sum of ‘Minimum order size’ + ‘Price Tick’ should not exceed the quote token decimals.

So, for PLATY PUSAI the meme coin celebrating AI and blockchain technology with a 
decimal value of 6 and an initial liquidity supply of 3,000,000,000,000.000000
minimum order size 6 indicates that you may buy 0.000001
and a price ticker of 0 indicates that the value of 1 PLATY PUSAI is measured for the value expression

6+0=6 which is the number of decimal places in PLATY PUSAI making PLATY PUSAI very suitable for value expression against USDC which also has a decimal expression of 6


# install openbook-v2 on Linux Mint 20




