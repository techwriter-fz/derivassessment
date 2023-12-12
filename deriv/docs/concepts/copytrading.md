# Copy trading

Copy Trading allows a client (the Copier) to automatically copy the trades of another client (the Trader).

## Becoming a Trader
To become a Trader (i.e. to allow others to follow your trades), set the “allow_copiers” setting via the  [set settings](https://api.deriv.com/api-explorer#set_settings) call.

The Trader then creates a read-only API token and provides it to the Copier.

Enabling the allow_copiers setting will also make the [copytrading statistics](https://api.deriv.com/api-explorer#copytrading_statistics) call work. The statistics API call provides the information about an account (this is so that potential copiers have an idea about the trader’s past performance).

## Becoming a Copier
To become a copier, use the [copy start](https://api.deriv.com/api-explorer#copy_start) call. To stop copying, use the [copy stop](https://api.deriv.com/api-explorer#copy_stop) call.
