---
sidebar_position: 13
---

# Warehouse Products API

Warehouse Products API

`PrintfulStoreClient.warehouseProducts`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#tag/Warehouse-Products-API)

[**Source**](https://github.com/artT14/printful-sdk-js/blob/main/src/lib/warehouse-products.ts)

---

## Get a list of your warehouse products

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getWarehouseProducts)

Returns a list of warehouse products from your store

**Method**

`PrintfulStoreClient.warehouseProducts.getAllWarehouseProducts(query?: string, offset?: number, limit?: number)`

**Arguments**

*Optional* `query` - Filter by partial or full product name

*Optional* `offset` - Number of items per page (max 100)

*Optional* `limit` - Result set offset

**Example Usage:**

```js
// Soon to be added
```

## Get warehouse product data

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getWarehouseProduct)

Returns warehouse product data by ID

**Method**

`PrintfulStoreClient.warehouseProducts.getWarehouseProduct(id: number | string)`

**Arguments**

`id` - Product ID

**Example Usage:**

```js
// Soon to be added
```