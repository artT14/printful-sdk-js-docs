---
sidebar_position: 4
---

# Orders API

The Orders API allows you to create new orders and confirm them for fulfillment.

`PrintfulStoreClient.orders`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#tag/Orders-API)

[**Source**](https://github.com/artT14/printful-sdk-js/blob/main/src/lib/orders.ts)

---

## Get list of orders

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getOrders)

Returns list of order objects from your store

**Method**

`PrintfulStoreClient.orders.getAllOrders(offset?: number, limit?: number, status?: OrderStatus)`

**Arguments**

*Optional* `status` - Filter by order status

*Optional* `offset` -  Result set offset

*Optional* `limit` -  Number of items per page (max 100)

**Example Usage:**
```js
//Soon to be added
```

## Create a new order

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/createOrder)

Creates a new order and optionally submits it for fulfillment

**Method**

`PrintfulStoreClient.orders.createOrder(newOrder: Order, confirm?: boolean, update_existing?: boolean)`

**Arguments**

`newOrder` - information about new order

*Optional* `confirm` - Automatically submit the newly created order for fulfillment (skip the Draft phase)

*Optional* `update_existing` - Try to update existing order if an order with the specified external_id already exists

**Example Usage:**
```js
//Soon to be added
```

## Get order data

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getOrderById)

Returns order data by ID or External ID.

**Method**

`PrintfulStoreClient.orders.getOrder(id: number | string)`

**Arguments**

`id` - Order ID (integer) or External ID (if prefixed with `@`)

**Example Usage:**
```js
//Soon to be added
```

## Cancel an order

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/cancelOrderById)

Cancels pending order or draft. Charged amount is returned to the store owner's credit card.

**Method**

`PrintfulStoreClient.orders.cancelOrder(id: number | string)`

**Arguments**

`id` - Order ID (integer) or External ID (if prefixed with `@`)

**Example Usage:**
```js
//Soon to be added
```

## Update order data

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/updateOrderById)

Updates unsubmitted order and optionally submits it for the fulfillment.

**Method**

`PrintfulStoreClient.orders.updateOrder(id: number | string, orderData: Order, confirm?: boolean)`

**Arguments**

`id` - Order ID (integer) or External ID (if prefixed with `@`)
`orderData` - Update information about the order
*Optional* `confirm` - Automatically submit the newly created order for fulfillment (skip the Draft phase)

**Example Usage:**
```js
//Soon to be added
```

## Confirm draft for fulfillment

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/confirmOrderById)

Approves for fulfillment an order that was saved as a draft. Store owner's credit card is charged when the order is submitted for fulfillment.

**Method**

`PrintfulStoreClient.orders.confirmOrder(id: number | string)`

**Arguments**

`id` - Order ID (integer) or External ID (if prefixed with `@`)

**Example Usage:**
```js
//Soon to be added
```

## Estimate order costs

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/estimateOrderCosts)

Calculates the estimated order costs including item costs, print costs (back prints, inside labels etc.), shipping and taxes

**Method**

`PrintfulStoreClient.orders.estimateOrderCost(orderData: Order)`

**Arguments**

`orderData` - Information on order for which estimate will be returned

**Example Usage:**
```js
//Soon to be added
```