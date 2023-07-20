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

`PrintfulStoreClient.mockupGenerator.createMockupTask()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/createGeneratorTask)

Creates an asynchronous mockup generation task. Generation result can be retrieved using `PrintfulStoreClient.mockupGenerator.getMockupTaskResult()`



## Retrieve product variant printfiles

`PrintfulStoreClient.mockupGenerator.getProductVariantPrintFiles()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getPrintfiles)

List of printfiles available for products variants. Printfile indicates what file resolution should be used to create a mockup or submit an order.



## Mockup generation task result

`PrintfulStoreClient.mockupGenerator.getMockupTaskResult()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getTask)

Returns asynchronous mockup generation task result. If generation task is completed, it will contain a list of generated mockups.



## Layout templates

`PrintfulStoreClient.mockupGenerator.getLayoutTemplates()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getTemplates)

Retrieve list of templates that can be used for client-side positioning.