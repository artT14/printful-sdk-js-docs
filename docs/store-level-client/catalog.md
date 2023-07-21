---
sidebar_position: 2
---

# Catalog API

Catalog API allows receiving data for a substantial catalog of blank Products and Variants.

`PrintfulStoreClient.catalog`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#tag/Catalog-API)

[**Source**](https://github.com/artT14/printful-sdk-js/blob/main/src/lib/catalog.ts)

---

## Get Products

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/getProducts)

Returns list of blank Products available in the Printful Catalog.

**Method**

`PrintfulStoreClient.catalog.getAllProducts(category_id?: string)`

**Arguments**

`category_id` - A comma-separated list of Category IDs of the Products that are to be returned

**Example Usage:**

```js
import {createPrintfulStoreClient} from "printful-sdk-js";

// ASYNC BLOCK
const client = createPrintfulStoreClient("STORE_TOKEN");
const {result: products, error} = await client.catalog.getAllProducts();
// ASYNC BLOCK

if(error){
	console.error(error);
}else{
	console.table(products);
}
```

## Get Variant

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/getVariantById)

Returns information about a specific Variant and its Product.

**Method**

`PrintfulStoreClient.catalog.getVariant(id: number)`

**Arguments**

`id` - Product ID.

**Example Usage:**

```js
import {createPrintfulStoreClient} from "printful-sdk-js";

// ASYNC BLOCK
const client = createPrintfulStoreClient("STORE_TOKEN");
const {result: variant, error} = await client.catalog.getVariant(4018);
// ASYNC BLOCK

if(error){
	console.error(error);
}else{
	console.log(variant);
}
```

## Get Product

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/getProductById)

Returns information about a specific product and a list of variants for this product.

**Method**

`PrintfulStoreClient.catalog.getProduct(id: number)`

**Arguments**

`id` - Product ID.

**Example Usage:**

```js
import {createPrintfulStoreClient} from "printful-sdk-js";

// ASYNC BLOCK
const client = createPrintfulStoreClient("STORE_TOKEN");
const {result: product, error} = await client.catalog.getProduct(71);
// ASYNC BLOCK

if(error){
	console.error(error);
}else{
	console.log(product);
}
```

## Get Product Size Guide

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/getProductSizeGuideById)

Returns information about the size guide for a specific product.

**Method**

`PrintfulStoreClient.catalog.getSize()`

**Arguments**

`id` - Product ID.

**Example Usage:**

```js
import {createPrintfulStoreClient} from "printful-sdk-js";

// ASYNC BLOCK
const client = createPrintfulStoreClient("STORE_TOKEN");
const {result: sizeGuide, error} = await client.catalog.getSize(71);
// ASYNC BLOCK

if(error){
	console.error(error);
}else{
	console.log(sizeGuide);
}
```

## Get Categories

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/getCategories)

Returns list of Catalog Categories available in the Printful.

**Method**

`PrintfulStoreClient.catalog.getAllCategories()`

**Arguments**

*None*

**Example Usage:**

```js
import {createPrintfulStoreClient} from "printful-sdk-js";

// ASYNC BLOCK
const client = createPrintfulStoreClient("STORE_TOKEN");
const {result: categories, error} = await client.catalog.getCategories();
// ASYNC BLOCK

if(error){
	console.error(error);
}else{
	console.log(categories);
}
```

## Get Category

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/getCategoryById)

Returns information about a specific category.

**Method**

`PrintfulStoreClient.catalog.getCategory(id: number)`

**Arguments**

`id` - Category ID

**Example Usage:**

```js
import {createPrintfulStoreClient} from "printful-sdk-js";

// ASYNC BLOCK
const client = createPrintfulStoreClient("STORE_TOKEN");
const {result: category, error} = await client.catalog.getCategory();
// ASYNC BLOCK

if(error){
	console.error(error);
}else{
	console.log(category);
}
```