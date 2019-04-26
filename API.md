
<p align="center">
  <a href="https://orionprotocol.io">
    <img src="https://res.cloudinary.com/dnbcgedbu/image/upload/v1556261195/photo_2019-04-26_08-42-57.jpg" />
  </a>
</p>

<h3 align="center">Orion Broker API Documentation</h3>

## API Functions

- [API Functions](#api-functions)
- [Open orders](#open-orders)
	- [HTTP Request](#http-request)
- [Order history](#order-history)
	- [HTTP Request](#http-request-1)
- [Cancel order](#cancel-order)
	- [HTTP Request](#http-request-2)
	- [Query Parameters](#query-parameters)
- [Order](#order)
	- [HTTP Request](#http-request-3)
	- [Query Parameters](#query-parameters-1)
- [Trade](#trade)
	- [HTTP Request](#http-request-4)
	- [Query Parameters](#query-parameters-2)
- [Order1](#order1)
	- [HTTP Request](#http-request-5)

## Open orders

This endpoint retrieves all open orders

### HTTP Request

`GET http://example.com/api/openorders`

## Order history

This endpoint retrieves the orders history

### HTTP Request

`GET http://example.com/api/orderhistory`

## Cancel order

This endpoint cancel an order.

### HTTP Request

`GET http://example.com/api/cancelorder`

### Query Parameters

Parameter | Default | Description | Value
-|-|-|-
id || Order id| Number
submitId || Submitted order id. This value is ignored if an id is specified. | Number

## Order

This endpoint create an order.

### HTTP Request

`GET http://example.com/api/order`

### Query Parameters

Parameter | Default | Description | Value
-|-|-|-
side || Order side | String, e.g. - BUY / SELL
symbol || Trading pair | String, e.g. - BTC_ETH
exchange || Id of the exchange | Number
ordType | "LIMIT" | Order type| String, e.g. - LIMIT
price || Price | Number
subOrdQty || Order quantity | Number
ordId || Order id |Number
subOrdId |||Number

## Trade

This endpoint create a trade.

### HTTP Request

`GET http://example.com/api/trade`

### Query Parameters

Parameter | Default | Description | Value
-|-|-|-
exchange || Id of the exchange| Number
ordId || Exchange Order id | Number
tradeId || Trade id | Number
price || Price | Number
qty || Order quantity | Number
status |||

## Order1

This endpoint retrieves the first filled order

### HTTP Request

`GET http://example.com/api/order1`