---
sidebar_position: 10
---

# Webhook API

Webhooks are an API feature that allows your system to receive notifications about certain events. To set up webhooks, use API requests described below.

`PrintfulStoreClient.webhook`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#tag/Webhook-API)

[**Source**](https://github.com/artT14/printful-sdk-js/blob/main/src/lib/webhook.ts)

---

## Get webhook configuration

`PrintfulStoreClient.webhook.getWebhookConfig()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getWebhooks)

Returns configured webhook URL and list of webhook event types enabled for the store



## Set up webhook configuration

`PrintfulStoreClient.webhook.setWebhookConfig()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/createWebhook)

Use this endpoint to enable a webhook URL for a store and select webhook event types that will be sent to this URL.



## Disable webhook support

`PrintfulStoreClient.webhook.disableWebhookSupport()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/disableWebhook)

Removes the webhook URL and all event types from the store.