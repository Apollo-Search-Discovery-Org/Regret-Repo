# Cart Viewed

### 

## Javascript Code
```js
window.appEventData000 = window.appEventData000 || [];
appEventData000.push({
  "event": "Cart Viewed",
    "cart": {
        "cartID": "<cartID>",
        "item": [
            {
                "productInfo": {
                    "isBackOrdered": "<isBackOrdered>"
                }
            }
        ]
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|cartID|string|Back-end identifier for a shopping cart|12345, 435678, 34567, XCV456, XCV876|||||||
|isBackOrdered|boolean|Boolean flag indicating that an inventoried product is on backorder|TRUE, FALSE|||||||
