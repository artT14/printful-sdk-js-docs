---
sidebar_position: 2
---
# Creating a client

Printful offers 2 levels of access for a client, a **Store client** and an **Account client**.

*Currently the SDK only offers support for <strong>Store Clients</strong>. Support for <strong>Account Clients</strong> is WIP🚧.*

## Store Level Client
To instantiate a client, do the following:

```js
import {createPrintfulStoreClient} from "printful-sdk-js";

const STORE_TOKEN = "YOUR STORE TOKEN";

const client = createPrintfulStoreClient(STORE_TOKEN);
```

### Getting an access token

Read the following guide on Prinful API Docs on [Authentication](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#tag/Authorization).

> **IMPORTANT NOTE:** It is advised to keep your API keys safe by storing them in a .env file and importing it into your project using a tool like **[dotenv](https://www.npmjs.com/package/dotenv)** or any equivalent you may have available in your project.

### Submodules of Store Client

After instantiation, `client` offers a multitude of submodules that correspond to the sub-APIs as described by the Printful API Documentation.

Below is a table mapping the SDK submodules to their respective sub-APIs.
> **NOTE:** Parts of the HTTP responses are abstracted away by the SDK. If you would like to investigate further, you are welcome to dive into the *[source code](https://github.com/artT14/printful-sdk-js)*.  


| SDK Submodule | Printful Sub-API |
|-----------|---------|
|`client.oauth`|[OAuth API](https://developers.printful.com/docs/?_gl=1*1f9fewg*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTcyMjgxMS4yNi4wLjE2ODk3MjI4MTEuNjAuMC4w#tag/OAuth-API)|
|`client.catalog`|[Catalog API](https://developers.printful.com/docs/?_gl=1*1f9fewg*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTcyMjgxMS4yNi4wLjE2ODk3MjI4MTEuNjAuMC4w#tag/Catalog-API)|
|`client.products`|[Products API](https://developers.printful.com/docs/?_gl=1*1f9fewg*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTcyMjgxMS4yNi4wLjE2ODk3MjI4MTEuNjAuMC4w#tag/Products-API)|
|`client.orders`|[Orders API](https://developers.printful.com/docs/?_gl=1*1f9fewg*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTcyMjgxMS4yNi4wLjE2ODk3MjI4MTEuNjAuMC4w#tag/Orders-API)|
|`client.fileLibrary`|[File Library API](https://developers.printful.com/docs/?_gl=1*1f9fewg*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTcyMjgxMS4yNi4wLjE2ODk3MjI4MTEuNjAuMC4w#tag/File-Library-API)|
|`client.shippingRate`|[Shipping Rate API](https://developers.printful.com/docs/?_gl=1*1f9fewg*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTcyMjgxMS4yNi4wLjE2ODk3MjI4MTEuNjAuMC4w#tag/Shipping-Rate-API)|
|`client.ecommerceSync`|[Ecommerce Platform Sync API](https://developers.printful.com/docs/?_gl=1*1f9fewg*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTcyMjgxMS4yNi4wLjE2ODk3MjI4MTEuNjAuMC4w#tag/Ecommerce-Platform-Sync-API)|
|`client.countryCodes`|[Country/State Code API](https://developers.printful.com/docs/?_gl=1*1f9fewg*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTcyMjgxMS4yNi4wLjE2ODk3MjI4MTEuNjAuMC4w#tag/CountryState-Code-API)|
|`client.taxRate`|[Tax Rate API](https://developers.printful.com/docs/?_gl=1*1f9fewg*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTcyMjgxMS4yNi4wLjE2ODk3MjI4MTEuNjAuMC4w#tag/Tax-Rate-API)|
|`client.webhook`|[Webhook API](https://developers.printful.com/docs/?_gl=1*1f9fewg*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTcyMjgxMS4yNi4wLjE2ODk3MjI4MTEuNjAuMC4w#tag/Webhook-API)|
|`client.storeInformation`|[Store Information API](https://developers.printful.com/docs/?_gl=1*1f9fewg*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTcyMjgxMS4yNi4wLjE2ODk3MjI4MTEuNjAuMC4w#tag/Store-Information-API)|
|`client.mockupGenerator`|[Mockup Generator API](https://developers.printful.com/docs/?_gl=1*1f9fewg*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTcyMjgxMS4yNi4wLjE2ODk3MjI4MTEuNjAuMC4w#tag/Mockup-Generator-API)|
|`client.warehouseProducts`|[Warehouse Products API](https://developers.printful.com/docs/?_gl=1*1f9fewg*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTcyMjgxMS4yNi4wLjE2ODk3MjI4MTEuNjAuMC4w#tag/Warehouse-Products-API)|
|`client.reports`|[Reports API](https://developers.printful.com/docs/?_gl=1*1f9fewg*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTcyMjgxMS4yNi4wLjE2ODk3MjI4MTEuNjAuMC4w#tag/Reports-API)|
|`client.approvalSheets`|[Approval Sheets API](https://developers.printful.com/docs/?_gl=1*1f9fewg*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTcyMjgxMS4yNi4wLjE2ODk3MjI4MTEuNjAuMC4w#tag/Approval-Sheets-API)|


## Account Level Client
*Support for <strong>Account Clients</strong> is WIP🚧.*


