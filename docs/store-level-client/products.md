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

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/getSyncProducts)

Returns a list of Sync Product objects from your custom Printful store.

**Method**

`PrintfulStoreClient.products.getAllSyncProducts(offset?: number, limit?: number, category_id?: string)`

**Arguments**

*Optional* `offset` - Offset for Paging

*Optional* `limit` - Limit items for Paging

*Optional* `category_id` - A comma-separated list of Category IDs of the Products that are to be returned

**Example Usage:**

```js
import {createPrintfulStoreClient} from "printful-sdk-js";

// ASYNC BLOCK
const client = createPrintfulStoreClient("STORE_TOKEN");
const {result: products, paging, error} = await client.products.getAllSyncProducts();
// ASYNC BLOCK

if(error){
	console.error(error);
}else{
	console.log(products);
	console.log(paging);
}
```

## Get a Sync Product

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/getSyncProductById)

Get information about a single Sync Product and its Sync Variants.

**Method**

`PrintfulStoreClient.products.getSyncProduct(id: number | string)`

**Argument**

`id` - Sync Product ID (integer) or External ID (if prefixed with `@`)

**Example Usage:**

```js
import {createPrintfulStoreClient} from "printful-sdk-js";

// ASYNC BLOCK
const client = createPrintfulStoreClient("STORE_TOKEN");
const {result: product, error} = await client.products.getSyncProduct(314179759);
// ASYNC BLOCK

if(error){
	console.error(error);
}else{
	console.log(product);
}
```



## Create a new Sync Product

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/createSyncProduct)

Creates a new Sync Product together with its Sync Variants. [See Examples](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#section/Products-API-examples/Create-a-new-Sync-Product)

**Method**

`PrintfulStoreClient.products.createSyncProduct(sync_product: SyncProduct, sync_variants: Array<SyncVariant>)`

**Arguments**

`sync_product` - Information about the SyncProduct

`sync_variants` - Information about the Sync Variants

**Example Usage**

```js
import {createPrintfulStoreClient} from "printful-sdk-js";
import { SYNC_PRODUCT, SYNC_VARIANTS } from "./data/products";

// ASYNC BLOCK
const client = createPrintfulStoreClient("STORE_TOKEN");
const {result: product, error} = await client.products.createSyncProduct(SYNC_PRODUCT, SYNC_VARIANTS);
// ASYNC BLOCK

if(error){
	console.error(error);
}else{
	console.log(product);
}
```

Where `./data/products` contains the following data:

```js
export const SYNC_PRODUCT = {
	"name": "API product Bella",
	"thumbnail": "https://example.com/image.jpg"
}

export const SYNC_VARIANTS = [
	{
		"retail_price": "21.00",
		"variant_id": 4011,
		"files": [
			{
				"url": "https://example.com/image.jpg"
			},
			{
				"type": "back",
				"url": "https://example.com/image.jpg"
			}
		]
	},
	{
		"retail_price": "21.00",
		"variant_id": 4012,
		"files": [
			{
				"url": "https://example.com/image.jpg"
			},
			{
				"type": "back",
				"url": "https://example.com/image.jpg"
			}
		]
	}
]
```

## Delete a Sync Product

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/deleteSyncProduct)

Deletes a Sync Product with all of its Sync Variants.

**Method**

`PrintfulStoreClient.products.deleteSyncProduct(id: number | string)`

**Arguments**

`id` - Sync Product ID (integer) or External ID (if prefixed with `@`)

**Example Usage:**

```js
import {createPrintfulStoreClient} from "printful-sdk-js";
import { SYNC_PRODUCT, SYNC_VARIANTS } from "./data/products";

// ASYNC BLOCK
const client = createPrintfulStoreClient("STORE_TOKEN");
const {result: product} = await client.products.createSyncProduct(SYNC_PRODUCT, SYNC_VARIANTS);
const {result: deletedProduct, error} = await client.products.deleteSyncProduct(product.id)
// ASYNC BLOCK

if(error){
	console.error(error);
}else{
	console.log(deletedProduct);
}
```

Where `./data/products` contains the following data:

```js
export const SYNC_PRODUCT = {
	"name": "API product Bella",
	"thumbnail": "https://example.com/image.jpg"
}

export const SYNC_VARIANTS = [
	{
		"retail_price": "21.00",
		"variant_id": 4011,
		"files": [
			{
				"url": "https://example.com/image.jpg"
			},
			{
				"type": "back",
				"url": "https://example.com/image.jpg"
			}
		]
	},
	{
		"retail_price": "21.00",
		"variant_id": 4012,
		"files": [
			{
				"url": "https://example.com/image.jpg"
			},
			{
				"type": "back",
				"url": "https://example.com/image.jpg"
			}
		]
	}
]
```



## Modify a Sync Product

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/updateSyncProduct)

Modifies an existing Sync Product with its Sync Variants.

**Method**

`PrintfulStoreClient.products.modifySyncProduct(id: number | string, sync_product?: OptionalSyncProduct, sync_variants?: Array<OptionalSyncVariant>)`

**Arguments**

`id` - Sync Product ID (integer) or External ID (if prefixed with `@`)

`sync_product` - Information about the SyncProduct

`sync_variants` - Information about the Sync Variants

**Example Usage:**

```js
import { createPrintfulStoreClient } from "printful-sdk-js";
import { SYNC_PRODUCT, SYNC_PRODUCT_2, SYNC_VARIANTS, MODIFIED_SYNC_VARIANT } from "./data/products";

// ASYNC BLOCK
const client = createPrintfulStoreClient("STORE_TOKEN");
const {result: {id}} = await client.products.createSyncProduct(SYNC_PRODUCT, SYNC_VARIANTS);
const {result: product, error} = await client.products.modifySyncProduct(id, SYNC_PRODUCT_2, SYNC_VARIANTS);
// ASYNC BLOCK

if(error){
	console.error(error);
}else{
	console.log(product);
}
```

Where `./data/products` contains the following data:

```js
export const SYNC_PRODUCT = {
	"name": "API product Bella",
	"thumbnail": "https://example.com/image.jpg"
}

export const SYNC_PRODUCT_2 = {
	"name": "API product Bella Modified",
	"thumbnail": "https://example.com/image.jpg"
}

export const SYNC_VARIANTS = [
	{
		"retail_price": "21.00",
		"variant_id": 4011,
		"files": [
			{
				"url": "https://example.com/image.jpg"
			},
			{
				"type": "back",
				"url": "https://example.com/image.jpg"
			}
		]
	},
	{
		"retail_price": "21.00",
		"variant_id": 4012,
		"files": [
			{
				"url": "https://example.com/image.jpg"
			},
			{
				"type": "back",
				"url": "https://example.com/image.jpg"
			}
		]
	}
]

export const MODIFIED_SYNC_VARIANT = {
	"retail_price": "420.69",
	"variant_id": 4013,
	"files": [
		{
			"url": "https://example.com/image.jpg"
		},
		{
			"type": "back",
			"url": "https://example.com/image.jpg"
		}
	]
}
```



## Get a Sync Variant

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/getSyncVariantById)

Get information about a single Sync Variant.

**Method**

`PrintfulStoreClient.products.getSyncVariant(id: number | string)`

**Arguments**

`id` -  Sync Variant ID (integer) or External ID (if prefixed with `@`)

**Example Usage:**
```js
import { createPrintfulStoreClient } from "printful-sdk-js";

// ASYNC BLOCK
const client = createPrintfulStoreClient("STORE_TOKEN");
const {result: products} = await client.products.getAllSyncProducts();
const {result: {sync_variants}} = await client.products.getSyncProduct(products[0].id);
const {result: variant, error, code} = await client.products.getSyncVariant(sync_variants[0].id);
// ASYNC BLOCK

if(error){
	console.error(error);
}else{
	console.log(variant);
}
```


## Delete a Sync Variant

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/deleteSyncVariant)

Deletes a single Sync Variant.

**Method**

`PrintfulStoreClient.products.deleteSyncVariant(id: number | string)`

**Arguments**

`id` - Sync Variant ID (integer) or External ID (if prefixed with `@`)

**Example Usage:**

```js
import { createPrintfulStoreClient } from "printful-sdk-js";
import { SYNC_PRODUCT, SYNC_VARIANTS } from "./data/products";

// ASYNC BLOCK
const client = createPrintfulStoreClient("STORE_TOKEN");
const {result: {id}} = await client.products.createSyncProduct(SYNC_PRODUCT, SYNC_VARIANTS);
const {result: {sync_variants}} = await client.products.getSyncProduct(id);
const {result: variant, error, code} = await client.products.deleteSyncVariant(sync_variants[0].id);
// ASYNC BLOCK

if(error){
	console.error(error);
}else{
	console.log(variant);
}
```

Where `./data/products` contains the following data:

```js
export const SYNC_PRODUCT = {
	"name": "API product Bella",
	"thumbnail": "https://example.com/image.jpg"
}

export const SYNC_VARIANTS = [
	{
		"retail_price": "21.00",
		"variant_id": 4011,
		"files": [
			{
				"url": "https://example.com/image.jpg"
			},
			{
				"type": "back",
				"url": "https://example.com/image.jpg"
			}
		]
	},
	{
		"retail_price": "21.00",
		"variant_id": 4012,
		"files": [
			{
				"url": "https://example.com/image.jpg"
			},
			{
				"type": "back",
				"url": "https://example.com/image.jpg"
			}
		]
	}
]
```

## Modify a Sync Variant

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/updateSyncVariant)

Modifies an existing Sync Variant.

**Method**

`PrintfulStoreClient.products.modifySyncVariant(id: number | string, sync_variant: OptionalSyncVariant)`

**Arguments**

`id` - Sync Variant ID (integer) or External ID (if prefixed with `@`)

`sync_variant` - Information about the Sync Variant

**Example Usage:**

```js
import { createPrintfulStoreClient } from "printful-sdk-js";
import { SYNC_PRODUCT, SYNC_VARIANTS, MODIFIED_SYNC_VARIANT } from "./data/products";

// ASYNC BLOCK
const client = createPrintfulStoreClient("STORE_TOKEN");
const {result: {id}} = await client.products.createSyncProduct(SYNC_PRODUCT, SYNC_VARIANTS);
const {result: {sync_variants}} = await client.products.getSyncProduct(id);
const {result: variant, error, code} = await client.products.modifySyncVariant(sync_variants[0].id, MODIFIED_SYNC_VARIANT);
// ASYNC BLOCK

if(error){
	console.error(error);
}else{
	console.log(variant);
}
```

Where `./data/products` contains the following data:

```js
export const SYNC_PRODUCT = {
	"name": "API product Bella",
	"thumbnail": "https://example.com/image.jpg"
}

export const SYNC_VARIANTS = [
	{
		"retail_price": "21.00",
		"variant_id": 4011,
		"files": [
			{
				"url": "https://example.com/image.jpg"
			},
			{
				"type": "back",
				"url": "https://example.com/image.jpg"
			}
		]
	},
	{
		"retail_price": "21.00",
		"variant_id": 4012,
		"files": [
			{
				"url": "https://example.com/image.jpg"
			},
			{
				"type": "back",
				"url": "https://example.com/image.jpg"
			}
		]
	}
]

export const MODIFIED_SYNC_VARIANT = {
	"retail_price": "420.69",
	"variant_id": 4013,
	"files": [
		{
			"url": "https://example.com/image.jpg"
		},
		{
			"type": "back",
			"url": "https://example.com/image.jpg"
		}
	]
}
```

## Create a new Sync Variant

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/createSyncVariant)

Creates a new Sync Variant for an existing Sync Product. [See Examples](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#section/Products-API-examples/Create-a-new-Sync-Variant)

**Method**

`PrintfulStoreClient.products.createSyncVariant(id: number | string, sync_variant: SyncVariant)`

**Arguments**

`id` - Sync Product ID (integer) or External ID (if prefixed with `@`)

`sync_variant` - Information about the Sync Variant

**Example Usage:**

```js
import { createPrintfulStoreClient } from "printful-sdk-js";
import { SYNC_PRODUCT, SYNC_VARIANTS, NEW_SYNC_VARIANT } from "./data/products";

// ASYNC BLOCK
const client = createPrintfulStoreClient("STORE_TOKEN");
const {result: product} = await client.products.createSyncProduct(SYNC_PRODUCT, SYNC_VARIANTS);
const {result: variant, error, code} = await client.products.createSyncVariant(product.id, NEW_SYNC_VARIANT);
// ASYNC BLOCK

if(error){
	console.error(error);
}else{
	console.log(variant);
}
```

Where `./data/products` contains the following data:

```js
export const SYNC_PRODUCT = {
	"name": "API product Bella",
	"thumbnail": "https://example.com/image.jpg"
}

export const SYNC_VARIANTS = [
	{
		"retail_price": "21.00",
		"variant_id": 4011,
		"files": [
			{
				"url": "https://example.com/image.jpg"
			},
			{
				"type": "back",
				"url": "https://example.com/image.jpg"
			}
		]
	},
	{
		"retail_price": "21.00",
		"variant_id": 4012,
		"files": [
			{
				"url": "https://example.com/image.jpg"
			},
			{
				"type": "back",
				"url": "https://example.com/image.jpg"
			}
		]
	}
]

export const NEW_SYNC_VARIANT = {
	"retail_price": "420.69",
	"variant_id": 4013,
	"files": [
		{
			"url": "https://example.com/image.jpg"
		},
		{
			"type": "back",
			"url": "https://example.com/image.jpg"
		}
	]
}
```
