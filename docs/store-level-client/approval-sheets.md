---
sidebar_position: 14
---

# Approval Sheets API

Approval Sheets API

`PrintfulStoreClient.approvalSheets`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#tag/Approval-Sheets-API)

[**Source**](https://github.com/artT14/printful-sdk-js/blob/main/src/lib/approval-sheets.ts)

---

## Retrieve a list of approval sheets

`PrintfulStoreClient.approvalSheets.getApprovalSheets()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getApprovalSheets)

Retrieve a list of approval sheets confirming suggested changes to files of on hold orders.



## Approve a design

`PrintfulStoreClient.approvalSheets.approveDesign()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/approveDesign)

Uses the confirm hash of an approval sheet to approve a design and remove the hold on an order




## Submit changes to an approval sheet

`PrintfulStoreClient.approvalSheets.changeApprovalSheet()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/submitApprovalSheetChanges)

Use this to submit alternative changes to a design that has an approval sheet