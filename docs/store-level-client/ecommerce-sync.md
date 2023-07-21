---
sidebar_position: 7
---

# Ecommerce Platform Sync API

The ecommerce platform sync API allows you to automatically assign Printful products and print files to the products in your online store (Shopify, Woocommerce, etc.) that is linked to Printful.

`PrintfulStoreClient.ecommerceSync`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#tag/Ecommerce-Platform-Sync-API)

[**Source**](https://github.com/artT14/printful-sdk-js/blob/main/src/lib/ecommerce-sync.ts)

---

## Get list of Sync Products

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getStoreSyncProducts)

Returns list of Sync Product objects from your store.

**Method**

`PrintfulStoreClient.ecommerceSync.getAllEcommProducts(offset?: number, limit?: number, status?: Status, search?: string)`

**Arguments**

*Optional* `offset` - Result set offset
*Optional* `limit` - Number of items per page (max 100)
*Optional* `status` - Filter by item status (synced/unsynced/all). If only some of the variants are synced,the product is returned by both unsynced and synced filters
*Optional* `search` - Product search needle

**Example Usage:**

```js
// Soon to be added
```


## Get a Sync Product

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getStoreSyncProductById)

Get information about a single Sync Product and its Sync Variants

**Method**

`PrintfulStoreClient.ecommerceSync.getEcommProduct(id: number | string)`

**Arguments**

`id` - Sync Product ID (integer) or External ID (if prefixed with `@`)

**Example Usage:**

```js
// Soon to be added
```

## Delete a Sync Product

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/deleteStoreSyncProduct)

Deletes a Sync Product with all of its Sync Variants

**Method**

`PrintfulStoreClient.ecommerceSync.deleteEcommProduct(id: number | string)`

**Arguments**

`id` - Sync Product ID (integer) or External ID (if prefixed with `@`)

**Example Usage:**

```js
// Soon to be added
```

## Get a Sync Variant

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getStoreSyncVariantById)

Get information about a single Sync Variant

**Method**

`PrintfulStoreClient.ecommerceSync.getEcommVariant(id: number | string)`

**Arguments**

`id` - Sync Variant ID (integer) or External ID (if prefixed with `@`)

**Example Usage:**

```js
// Soon to be added
```

## Modify a Sync Variant

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/updateStoreSyncVariant)

Modifies an existing Sync Variant.

**Method**

`PrintfulStoreClient.ecommerceSync.modifyEcommVariant(id: number | string, sync_variant_info: OptionalSyncVariant)`

**Arguments**

`id` - Sync Variant ID (integer) or External ID (if prefixed with `@`)
`sync_variant_info` - Information about the Sync Variant

**Example Usage:**

```js
// Soon to be added
```

## Delete a Sync Variant

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/deleteStoreSyncVariant)

Deletes configuraton information (variant_id, print files and options) and disables automatic order importing for this Sync Variant.

**Method**

`PrintfulStoreClient.ecommerceSync.deleteEcommVariant(id: number | string)`

**Arguments**

`id` - Sync Variant ID (integer) or External ID (if prefixed with `@`)

**Example Usage:**

```js
// Soon to be added
```