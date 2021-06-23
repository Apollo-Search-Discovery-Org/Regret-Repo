# Donation Completed

### 

## Javascript Code
```js
window.appEventData000 = window.appEventData000 || [];
appEventData000.push({
  "event": "Donation Completed",
    "donation": {
        "donationType": "<donationType>",
        "item": [
            {
                "donationAmount": "<donationAmount>"
            }
        ],
        "profile": {
            "address": {
                "stateProvince": "<stateProvince>"
            }
        },
        "transactionID": "<transactionID>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|donationAmount|string|String representation of the donation amount. Positive. Up to two decimal places for cents. No currency symbol.|200.00, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|donationType|string|Type of donation selected. |Tribute, General, Fundraiser|||||||
|stateProvince|string|The mailing state or province associated with the donation payment. |MO, GA, NB, ON|||||||
|transactionID|string|Unique identifier of the transaction. Max Length 20. Used as a key for upload of post transaction data. ||^[a-zA-Z0-9]{6,20}$|6|20||||
