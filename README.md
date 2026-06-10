<div align="center">

# Free Hourly Exchange Rate API

**A free, reliable, hourly-updated exchange rate API — committed to 10 years of free service.**

[![Website](https://img.shields.io/badge/Website-exchangerate.fun-2ea44f?style=for-the-badge)](https://www.exchangerate.fun/)
[![API](https://img.shields.io/badge/API-api.exchangerate.fun-blue?style=for-the-badge)](https://api.exchangerate.fun/latest)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](#license)
[![Updates](https://img.shields.io/badge/Updates-Hourly-orange?style=for-the-badge)]()
[![Free](https://img.shields.io/badge/Free-Forever-red?style=for-the-badge)]()

**[Website](https://www.exchangerate.fun/)** · **[Live API](https://api.exchangerate.fun/latest)** · **[中文文档](README_zh.md)**

</div>

---

## Overview

This project provides a **free, hourly-updated exchange rate API** for developers worldwide.

We solemnly commit to maintaining this API **free of charge for 10 years**, providing a stable and reliable source of exchange rate data for the developer community.

> Visit our website: **<https://www.exchangerate.fun/>**

## Table of Contents

- [Features](#features)
- [Quick Start](#quick-start)
- [API Reference](#api-reference)
- [Code Examples](#code-examples)
- [Maintenance Commitment](#maintenance-commitment)
- [Usage Guidelines](#usage-guidelines)
- [Contact](#contact)
- [License](#license)

## Features

| Feature | Description |
| :--- | :--- |
| **Free Forever** | Completely free with zero cost. No API key required. |
| **Hourly Updates** | Exchange rate data refreshed every hour. |
| **No Rate Limits** | No enforced request frequency limits — please use responsibly. |
| **170+ Currencies** | Comprehensive coverage including fiat, crypto, and precious metals. |
| **Public Welfare** | Built as a public service for the developer community. |
| **Long-Term Commitment** | Pledged to operate free for 10 years. |

## Quick Start

Get the latest USD exchange rates with a single request:

```bash
curl "https://api.exchangerate.fun/latest"
```

Or query against a different base currency:

```bash
curl "https://api.exchangerate.fun/latest?base=EUR"
```

That's it — no signup, no API key, no fuss.

## API Reference

### Endpoint

```
GET https://api.exchangerate.fun/latest
```

### Query Parameters

| Parameter | Type | Required | Default | Description |
| :--- | :--- | :--- | :--- | :--- |
| `base` | `string` | No | `USD` | The base currency code (ISO 4217). |

### Response Schema

| Field | Type | Description |
| :--- | :--- | :--- |
| `timestamp` | `integer` | Unix timestamp of when the rates were last updated. |
| `base` | `string` | The base currency code used for the rates. |
| `rates` | `object` | A map of currency codes to their exchange rate against the base. |

### Example Response

<details>
<summary><b>Click to expand sample JSON response</b></summary>

```json
{
  "timestamp": 1729598400,
  "base": "USD",
  "rates": {
    "AED": 3.67297,
    "AFN": 65.974197,
    "ALL": 91.1849,
    "AMD": 387.071853,
    "ANG": 1.802456,
    "AOA": 910.833667,
    "ARS": 983.2465,
    "AUD": 1.496047,
    "AWG": 1.8025,
    "AZN": 1.7,
    "BAM": 1.806335,
    "BBD": 2,
    "BDT": 119.511064,
    "BGN": 1.80702,
    "BHD": 0.376917,
    "BIF": 2903.915518,
    "BMD": 1,
    "BND": 1.315822,
    "BOB": 6.91117,
    "BRL": 5.6946,
    "BSD": 1,
    "BTC": 0.000014867307,
    "BTN": 84.085364,
    "BWP": 13.352174,
    "BYN": 3.272978,
    "BZD": 2.015904,
    "CAD": 1.383125,
    "CDF": 2841.015926,
    "CHF": 0.865771,
    "CLF": 0.034468,
    "CLP": 951.09,
    "CNH": 7.133518,
    "CNY": 7.1207,
    "COP": 4282.63,
    "CRC": 515.346789,
    "CUC": 1,
    "CUP": 25.75,
    "CVE": 101.838385,
    "CZK": 23.3413,
    "DJF": 178.094499,
    "DKK": 6.893964,
    "DOP": 60.208087,
    "DZD": 133.470425,
    "EGP": 48.6657,
    "ERN": 15,
    "ETB": 120.446576,
    "EUR": 0.924402,
    "FJD": 2.2337,
    "FKP": 0.770445,
    "GBP": 0.770445,
    "GEL": 2.72,
    "GGP": 0.770445,
    "GHS": 16.056486,
    "GIP": 0.770445,
    "GMD": 70,
    "GNF": 8627.105918,
    "GTQ": 7.734046,
    "GYD": 209.237762,
    "HKD": 7.772713,
    "HNL": 24.9163,
    "HRK": 6.964001,
    "HTG": 131.665362,
    "HUF": 370.056982,
    "IDR": 15569.299406,
    "ILS": 3.77846,
    "IMP": 0.770445,
    "INR": 84.077597,
    "IQD": 1310.188929,
    "IRR": 42102.5,
    "ISK": 138.02,
    "JEP": 0.770445,
    "JMD": 158.725497,
    "JOD": 0.709,
    "JPY": 150.8645,
    "KES": 129.01,
    "KGS": 85.5,
    "KHR": 4062.835806,
    "KMF": 455.150003,
    "KPW": 900,
    "KRW": 1378.971512,
    "KWD": 0.306422,
    "KYD": 0.833437,
    "KZT": 485.220568,
    "LAK": 21970.959528,
    "LBP": 89562.861135,
    "LKR": 293.282472,
    "LRD": 192.51994,
    "LSL": 17.587521,
    "LYD": 4.809997,
    "MAD": 9.898083,
    "MDL": 17.942137,
    "MGA": 4590.176245,
    "MKD": 56.873338,
    "MMK": 2098,
    "MNT": 3398,
    "MOP": 8.008478,
    "MRU": 39.773908,
    "MUR": 46.070002,
    "MVR": 15.36,
    "MWK": 1734.209227,
    "MXN": 19.928543,
    "MYR": 4.328,
    "MZN": 63.850001,
    "NAD": 17.587521,
    "NGN": 1643.34,
    "NIO": 36.804601,
    "NOK": 10.931453,
    "NPR": 134.53676,
    "NZD": 1.652387,
    "OMR": 0.384947,
    "PAB": 1,
    "PEN": 3.766445,
    "PGK": 3.999095,
    "PHP": 57.831501,
    "PKR": 277.730111,
    "PLN": 3.993455,
    "PYG": 7913.201145,
    "QAR": 3.646363,
    "RON": 4.597925,
    "RSD": 108.216,
    "RUB": 96.545975,
    "RWF": 1350.454986,
    "SAR": 3.75566,
    "SBD": 8.299327,
    "SCR": 13.787654,
    "SDG": 601.5,
    "SEK": 10.541506,
    "SGD": 1.3155,
    "SHP": 0.770445,
    "SLL": 20969.5,
    "SOS": 571.602794,
    "SRD": 33.215,
    "SSP": 130.26,
    "STD": 22281.8,
    "STN": 22.627255,
    "SVC": 8.750906,
    "SYP": 2512.53,
    "SZL": 17.583088,
    "THB": 33.480167,
    "TJS": 10.621202,
    "TMT": 3.5,
    "TND": 3.100453,
    "TOP": 2.3709,
    "TRY": 34.251598,
    "TTD": 6.794642,
    "TWD": 32.045002,
    "TZS": 2725.281338,
    "UAH": 41.333463,
    "UGX": 3665.686834,
    "USD": 1,
    "UYU": 41.570268,
    "UZS": 12806.488137,
    "VES": 39.132384,
    "VND": 25403.287269,
    "VUV": 118.722,
    "WST": 2.8,
    "XAF": 606.368281,
    "XAG": 0.02911912,
    "XAU": 0.00036603,
    "XCD": 2.70255,
    "XDR": 0.750315,
    "XOF": 606.368281,
    "XPD": 0.00093164,
    "XPF": 110.310559,
    "XPT": 0.00098368,
    "YER": 250.375001,
    "ZAR": 17.588317,
    "ZMW": 26.577941,
    "ZWL": 322
  }
}
```

</details>

## Code Examples

<details>
<summary><b>JavaScript / Node.js</b></summary>

```javascript
const response = await fetch('https://api.exchangerate.fun/latest?base=USD');
const data = await response.json();
console.log(`1 USD = ${data.rates.EUR} EUR`);
```

</details>

<details>
<summary><b>Python</b></summary>

```python
import requests

response = requests.get('https://api.exchangerate.fun/latest', params={'base': 'USD'})
data = response.json()
print(f"1 USD = {data['rates']['EUR']} EUR")
```

</details>

<details>
<summary><b>Go</b></summary>

```go
package main

import (
    "encoding/json"
    "fmt"
    "net/http"
)

type Response struct {
    Timestamp int64              `json:"timestamp"`
    Base      string             `json:"base"`
    Rates     map[string]float64 `json:"rates"`
}

func main() {
    resp, _ := http.Get("https://api.exchangerate.fun/latest?base=USD")
    defer resp.Body.Close()

    var data Response
    json.NewDecoder(resp.Body).Decode(&data)
    fmt.Printf("1 USD = %f EUR\n", data.Rates["EUR"])
}
```

</details>

<details>
<summary><b>PHP</b></summary>

```php
<?php
$response = file_get_contents('https://api.exchangerate.fun/latest?base=USD');
$data = json_decode($response, true);
echo "1 USD = {$data['rates']['EUR']} EUR";
```

</details>

## Maintenance Commitment

We solemnly pledge to maintain this API **free of charge for 10 years**. Throughout this period, we will strive to ensure the API's stability and the accuracy of its data.

## Usage Guidelines

- **Reasonable Use** — Please use the API responsibly and avoid unnecessary high-concurrency requests.
- **Public Welfare Nature** — This is a community service project; please help us keep it healthy and available for everyone.
- **Feedback & Contributions** — Suggestions, issues, and pull requests are warmly welcomed.

## Contact

If you have any questions or suggestions, please reach out:

- **Website**: <https://www.exchangerate.fun/>
- **Email**: <haxqer666@gmail.com>
- **GitHub**: [@haxqer](https://github.com/haxqer)

---

## License

This project is licensed under the **MIT License**.

<div align="center">

**[⬆ Back to Top](#free-hourly-exchange-rate-api)**

Made with care · Visit **[exchangerate.fun](https://www.exchangerate.fun/)**

</div>
