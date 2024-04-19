# react-native-barcode-sked

React Native component to generate barcodes. Uses
[JsBarcode](https://github.com/lindell/JsBarcode) for encoding of
data.
SKED forked this project to add support for svg since the original
library used ART which is no longer supported.


## Getting started

### Step 1

This library uses react-native-svg to draw vector graphics.

### Step 2

Install `react-native-barcode-sked`:

```shell
    npm install react-native-barcode-sked --save
```

### Step 3

Start using the component

```javascript
import Barcode from "react-native-barcode-sked";

<Barcode value="Hello World" format="CODE128" />;
```

You can find more info about the supported barcodes in the
[JsBarcode README](https://github.com/lindell/JsBarcode#supported-barcodes).

![demo](./images/example.png)

## Properties

| Property   | Description                                        |
| ---------- | -------------------------------------------------- |
| value      | What the barcode stands for (required).            |
| format     | Which barcode type to use (default: CODE128).      |
| width      | Width of a single bar (default: 2)                 |
| height     | Height of the barcode (default: 100)               |
| text       | Override text that is displayed.                   |
| lineColor  | Color of the bars and text (default: #000000)      |
| background | Background color of the barcode (default: #ffffff) |
| onError    | Handler for invalid barcode of selected format     |
