---
sidebar_position: 1
---
# Intro

## Getting Started

Get started by **installing the package**.

### What you'll need

- [Node.js](https://nodejs.org/en/download/) version 16.16 or above:
  - When installing Node.js, you are recommended to check all checkboxes related to dependencies.

## Installing the package

Install the package by running the following command:

```bash
npm i printful-sdk-js
```

You can type this command into Command Prompt, Powershell, Terminal, or any other integrated terminal of your code editor.

The command also installs all necessary dependencies you need to run printful-sdk-js.

## Example Usage

Basic Example in Code:

```js
import {createPrintfulStoreClient} from "printful-sdk-js";

const STORE_TOKEN = "YOUR STORE TOKEN";

const client = createPrintfulStoreClient(STORE_TOKEN);

// Must call within an async block
const {result: products, error} = await client.catalog.getAllProducts();

if (error){
	console.error(error);
}
else{
	console.table(products);
}
```

### Getting an access token

Read the following guide on Prinful API Docs on [Authentication](https://developers.printful.com/docs/?_gl=1*1sbmfdi*_ga*NDMzMTM2Mjk0LjE2ODcyMzU3MDc.*_ga_EZ4XVRL864*MTY4ODc3OTM1NC4xMi4xLjE2ODg3ODEwMzYuMTAuMC4w#tag/Authorization).

> **IMPORTANT NOTE:** It is advised to keep your API keys safe by storing them in a .env file and importing it into your project using a tool like **[dotenv](https://www.npmjs.com/package/dotenv)** or any equivalent you may have available in your project.