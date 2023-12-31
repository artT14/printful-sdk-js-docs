---
sidebar_position: 1
---

# OAuth API

OAuth API allows receiving data for token.

`PrintfulStoreClient.oauth`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#tag/OAuth-API)

[**Source**](https://github.com/artT14/printful-sdk-js/blob/main/src/lib/oauth.ts)

---

## Get scopes for token

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*89vqs2*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4OTgwNDI5My4zMC4wLjE2ODk4MDQyOTMuNjAuMC4w#operation/getScopes)

Returns a list of scopes associated with the token.

**Method**

`PrintfulStoreClient.oauth.getScopes()`

**Arguments**

*None*

**Example Usage:**

```js
import {createPrintfulStoreClient} from "printful-sdk-js";

const STORE_TOKEN = "YOUR STORE TOKEN";

const client = createPrintfulStoreClient(STORE_TOKEN);

// Must call within an async block
const {result, error, code} = await client.oauth.getScopes();
```


