---
sidebar_position: 3
---

# Products API

The Products API resource lets you create, modify and delete products in a Printful store based on the Manual orders / API platform

`PrintfulStoreClient.products`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#tag/Products-API)

[**Source**](https://github.com/artT14/printful-sdk-js/blob/main/src/lib/products.ts)

---

## Get Sync Products

`PrintfulStoreClient.products.getAllSyncProducts()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/getSyncProducts)

Returns a list of Sync Product objects from your custom Printful store.



## Create a new Sync Product

`PrintfulStoreClient.products.getSyncProduct()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/createSyncProduct)

Creates a new Sync Product together with its Sync Variants. [See Examples:](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#section/Products-API-examples/Create-a-new-Sync-Product)



## Get a Sync Product

`PrintfulStoreClient.products.createSyncProduct()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/getSyncProductById)

Get information about a single Sync Product and its Sync Variants.



## Delete a Sync Product

`PrintfulStoreClient.products.deleteSyncProduct()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/deleteSyncProduct)

Deletes a Sync Product with all of its Sync Variants.



## Modify a Sync Product

`PrintfulStoreClient.products.modifySyncProduct()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/updateSyncProduct)

Modifies an existing Sync Product with its Sync Variants.



## Get a Sync Variant

`PrintfulStoreClient.products.getSyncVariant()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/getSyncVariantById)

Get information about a single Sync Variant.



## Delete a Sync Variant

`PrintfulStoreClient.products.deleteSyncVariant()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/deleteSyncVariant)

Deletes a single Sync Variant.



## Modify a Sync Variant

`PrintfulStoreClient.products.modifySyncVariant()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/updateSyncVariant)

Modifies an existing Sync Variant.



## Create a new Sync Variant

`PrintfulStoreClient.products.createSyncVariant()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/createSyncVariant)

Creates a new Sync Variant for an existing Sync Product. [See Examples:](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#section/Products-API-examples/Create-a-new-Sync-Variant)