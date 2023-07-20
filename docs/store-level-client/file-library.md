---
sidebar_position: 5
---

# File Library API

You can use this API to directly add files to the library, and later use File IDs when creating orders.

`PrintfulStoreClient.fileLibrary`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#tag/File-Library-API)

[**Source**](https://github.com/artT14/printful-sdk-js/blob/main/src/lib/file-library.ts)

---

## Add a new file

`PrintfulStoreClient.fileLibrary.addFile()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/addFile)

Adds a new File to the library by providing URL of the file.



## Get file

`PrintfulStoreClient.fileLibrary.getFile()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/getFile)

Returns information about the given file.



## Return available thread colors from provided image URL

`PrintfulStoreClient.fileLibrary.getThreadColors()`

[**Printful API Reference**](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#operation/threadColors)

Returns colors in hexadecimal format.

Returned thread colors are matched as closely as possible to provided image colors.