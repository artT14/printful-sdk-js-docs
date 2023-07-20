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

`PrintfulStoreClient.ecommerceSync.getAllEcommProducts()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getStoreSyncProducts)

Returns list of Sync Product objects from your store.



## Get a Sync Product

`PrintfulStoreClient.ecommerceSync.getEcommProduct()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getStoreSyncProductById)

Get information about a single Sync Product and its Sync Variants



## Delete a Sync Product

`PrintfulStoreClient.ecommerceSync.deleteEcommProduct()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/deleteStoreSyncProduct)

Deletes a Sync Product with all of its Sync Variants



## Get a Sync Variant

`PrintfulStoreClient.ecommerceSync.()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getStoreSyncVariantById)

Get information about a single Sync Variant



## Modify a Sync Variant

`PrintfulStoreClient.ecommerceSync.getEcommVariant()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/updateStoreSyncVariant)

Modifies an existing Sync Variant.



## Delete a Sync Variant

`PrintfulStoreClient.ecommerceSync.modifyEcommVariant()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/deleteStoreSyncVariant)

Deletes configuraton information (variant_id, print files and options) and disables automatic order importing for this Sync Variant.