---
sidebar_position: 12
---

# Mockup Generator API

You can use this API to generate mockups for your products.

`PrintfulStoreClient.mockupGenerator`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#tag/Mockup-Generator-API)

[**Source**](https://github.com/artT14/printful-sdk-js/blob/main/src/lib/mockup-generator.ts)

---

## Create a mockup generation task

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/createGeneratorTask)

Creates an asynchronous mockup generation task. Generation result can be retrieved using

**Method**

`PrintfulStoreClient.mockupGenerator.createMockupTask(id: number, mockup_task: MockupTask)`

**Arguments**

`id` - Product ID. 

`mockup_task` - Mockup Task Info 

**Example Usage:**

```js
// Soon to be added
```

## Retrieve product variant printfiles

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getPrintfiles)

List of printfiles available for products variants. Printfile indicates what file resolution should be used to create a mockup or submit an order.

**Method**

`PrintfulStoreClient.mockupGenerator.getProductVariantPrintFiles(id: number, orientation?: Orientation, technique?: string)`

**Arguments**

`id` - Product ID. 

*Optional* `orientation` - Enum: "horizontal" "vertical", Optional orientation for wall art product printfiles. Allowed values: horizontal, vertical

*Optional* `technique` - Optional technique for product. This can be used in cases where product supports multiple techniques like DTG and embroidery

**Example Usage:**

```js
// Soon to be added
```

## Mockup generation task result

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getTask)

Returns asynchronous mockup generation task result. If generation task is completed, it will contain a list of generated mockups.

**Method**

`PrintfulStoreClient.mockupGenerator.getMockupTaskResult(task_key: string)`

**Arguments**

`task_key` - Task key retrieved when creating the generation task.

**Example Usage:**

```js
// Soon to be added
```

## Layout templates

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getTemplates)

Retrieve list of templates that can be used for client-side positioning.

**Method**

`PrintfulStoreClient.mockupGenerator.getLayoutTemplates(id: number, orientation?: Orientation, technique?: string)`

**Arguments**

`id` - Product ID. 
*Optional* `orientation` - Enum: "horizontal" "vertical", Optional orientation for wall art product printfiles. Allowed values: horizontal, vertical
*Optional* `technique` - Optional technique for product. This can be used in cases where product supports multiple techniques like DTG and embroidery


**Example Usage:**

```js
// Soon to be added
```