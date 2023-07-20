---
sidebar_position: 9
---

# Tax Rate API

You can use this API to gather information about tax rates.

`PrintfulStoreClient.taxRate`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#tag/Tax-Rate-API)

[**Source**](https://github.com/artT14/printful-sdk-js/blob/main/src/lib/tax-rate.ts)

---

## Get a list of countries for tax calculation

`PrintfulStoreClient.taxRate.getCountryTaxList()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getTaxCountries)

Retrieve state list that requires sales tax calculation



## Calculate tax rate

`PrintfulStoreClient.taxRate.calcTax()` ***Deprecated***

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/calculateTaxRates)

Calculates sales tax rate for given address if required