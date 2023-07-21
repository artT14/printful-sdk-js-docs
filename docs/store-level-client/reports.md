---
sidebar_position: 14
---

# Reports API

The Reports API lets you retrieve reports like the statistics related to the orders fulfilled for your stores.

`PrintfulStoreClient.reports`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#tag/Reports-API)

[**Source**](https://github.com/artT14/printful-sdk-js/blob/main/src/lib/reports.ts)

---

## Get statistics

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getStatistics)

Returns statistics for specified report types.

**Method**

`PrintfulStoreClient.reports.getStats(date_from: RawDateString , date_to: RawDateString, report_types: string, currency?: string)`

**Arguments**

`date_from` - The beginning of the period to get the statistics from (date in YYYY-MM-DD format). Example: 2022-08-01

`date_to` - The end of the period to get the statistics from (date in YYYY-MM-DD format). Example: 2022-08-31

`currency` - The currency (3-letter code) to return the statistics in. You can also specify display_currency as the value to get the statistics in the account's display currency. The store currency will be used by default. Example "USD"

`report_types` - A comma-separated list of report types to be retrieved. Example "sales_and_costs,profit"

**Example Usage:**

```js
// Soon to be added
```