---
sidebar_position: 11
---

# Store Information API

You can use this API to gather information about your stores.

`PrintfulStoreClient.storeInformation`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#tag/Store-Information-API)

[**Source**](https://github.com/artT14/printful-sdk-js/blob/main/src/lib/store-information.ts)

---

## Change packing slip

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/changePackingSlip)

Modifies packing slip information of the currently authorized Printful store.

**Method**

`PrintfulStoreClient.storeInformation.changePackingSlip(new_packing_slip: PackingSlip)`

**Arguments**

`new_packing_slip` - Packing slip information

**Example Usage:**

```js
// Soon to be added
```

## Get basic information about stores

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getStores)

Get basic information about stores depending on the token access level

**Method**

`PrintfulStoreClient.storeInformation.getAllStoresInfo(offset?: number, limit?: number)`

**Arguments**

*Optional* `offset` - Offset for query
*Optional* `limit`  - Limit for query

**Example Usage:**

```js
// Soon to be added
```

## Get basic information about a store

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getStore)

Get basic information about a store based on provided ID

**Method**

`PrintfulStoreClient.storeInformation.getStoreInfo(id: number)`

**Arguments**

`id` - Store ID

**Example Usage:**

```js
// Soon to be added
```