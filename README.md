# Receipt XML Test

## Overview

This project defines an XML and XSD structure for storing receipt information from different stores.  
The goal was to design one generic structure that can support multiple receipt formats and validate them against a common schema.

## Contents

### XML Files

- `prototyp.xml` – Prototype demonstrating all available constructs
- `willys.xml` – Example receipt from **Willys**
- `tempo.xml` – Example receipt from **Tempo**
- `bookshop.xml` – Example receipt from **Bookshop**
- `matboden.xml` – Example receipt from **Matboden**

### XSD Files

- `receipt.xsd` – Main XML Schema Definition
  - `common.xsd` – Shared components
  - `merchant.xsd` – Merchant details
  - `sale-identification.xsd` – SaleIdentification details
  - `order.xsd` – Order details 
  - `payment.xsd` – Payment details

## Resources

The overall structure and naming conventions were inspired by **Swedbank Pay NEXO Developer Documentation** and other related resources.  
Where possible, XML constructs were aligned with concepts from the referenced API to ensure clarity and alignment with industry standards.

* [Swedbank Pay Nexo Retailer – Payment Response](https://developer.swedbankpay.com/pax-terminal/Nexo-Retailer/Quick-guide/payment-response/#:~:text=Sample%20Payment%20Response%20for%20approved%20payment%20with%20physical%20payment%20card)
* [Swedbank Pay PAX Terminal – CustomerReceiptData](https://developer.swedbankpay.com/pax-terminal/NET/SwpTrmLib/Methods/essential/paymentasync/#:~:text=Test%20shop%0AH%C3%A4llesk%C3%A5ran,KVITTOT%0A%20%20%20%20%20%20KUNDENS%20EX.)
* [EMV Tag Decoders – Payment Card Tools](https://paymentcardtools.com/emv-tag-decoders/tvr)
* [XML Schema Definition Tutorial](https://youtu.be/DbHlO3GeLEA?si=yNOH-y4J4YYJ2YKh)

Additional references can be found in the `./sources/` directory.

---