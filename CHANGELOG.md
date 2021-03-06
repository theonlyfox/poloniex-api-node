# poloniex-api-node Changelog

All notable changes to this module are documented in this file.

poloniex-api-node module adheres to [Semantic Versioning](http://semver.org/).

## [1.8.2] - 2018-02-02
- Fixed: WebSocket keepAlive occasionally throws error 

## [1.8.1] - 2018-01-29
- Fixed: not possible to specify `paymentId`for method `withdraw`

## [1.8.0] - 2018-01-25
- Added: ability to set specific http.Agent for REST API calls and WebSocket connection (#53)

## [1.7.0] - 2018-01-09
- Changed: Examples updated
- Added: ability to pass in a nonce generating function

## [1.6.5] - 2017-11-21
- Fixed: Ignore unknown markets for ticker (WebSocket v2)
- Changed: Use dynamic market Ids (WebSocket v2) (#34)
- Added: Test for receiving 400 ticker messages

## [1.6.4] - 2017-11-20
- Fixed: STORJ currency added (#32)
- Added: allow passing `proxy` option to underlying request calls
- Added: Tests for node.js 9.x
- Added: Test to verify `orderBook` is first message type when subscribing to orderBook (WebSocket v2)

## [1.6.3] - 2017-10-16
- Fixed: minor documentation error
- Fixed: cannot subscribe to WebSocket (v2) before connection opens (#29)  

## [1.6.2] - 2017-09-08
- Fixed: custom string for 'User-Agent' in headers

## [1.6.0] - 2017-09-07
- Added: new WebSocket API (v2)

## [1.5.1] - 2017-09-04
- Added: WebSocket (push) API (v1)

## [1.4.0] - 2017-09-02
- Added: `limit` parameter for `returnTradeHistory` and `returnMyTradeHistory` methods
- Added: contributors to [README.md](README.md#contributors) (give credit where credit is due)  

## [1.3.1] - 2017-07-11
- Fixed: throw error when invalid parameters (#2)  

## [1.3.0] - 2017-07-02
- Added: Optional `keepAlive` parameter to constructor

## [1.2.0] - 2017-06-18
- Added: Promise support
- Changed: default socketTimeout changed from 10 seconds to 60 seconds

## [1.1.1] - 2017-05-08
- Fixed: Error handling for certain Poloniex error responses

## [1.1.0] - 2017-05-08
- Fixed: Error handling when Poloniex returns empty response
- Changed: HTTP default request timeout from 3 seconds to 10 seconds
- Added: Optional socket timeout parameter to constructor

## [1.0.2] - 2017-04-03
- Fixed: Return correct error message description for certain error codes (based on Poloniex API response)

## [1.0.1] - 2017-03-24
- Fixed: Return correct error message (based on recent Poloniex change of returning detailed error code)


## [1.0.0] - 2016-10-05

First release based on [https://github.com/premasagar/poloniex.js](https://github.com/premasagar/poloniex.js "https://github.com/premasagar/poloniex.js")

Notable differences:

- parameters adhere to Poloniex native API specification (e.g. currenncyPair instead of currencyA and currencyB)
- all optional parameters supported for all API methods
- improved handling of network errors
- improved handling of Poloniex API error codes and error code description
