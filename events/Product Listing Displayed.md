# Product Listing Displayed

### 

## Javascript Code
```js
window.appEventData000 = window.appEventData000 || [];
appEventData000.push({
  "event": "Product Listing Displayed",
    "listingDisplayed": {
        "listing": [
            {
                "isDisplayed": "<isDisplayed>",
                "itemPosition": "<itemPosition>",
                "price": {
                    "priceType": "<priceType>"
                },
                "productInfo": {
                    "brand": "<brand>",
                    "name": "<name>",
                    "productID": "<productID>",
                    "ratingAverage": "<ratingAverage>",
                    "sku": "<sku>",
                    "status": "<status>"
                }
            }
        ],
        "listingDriver": "<listingDriver>",
        "listingType": "<listingType>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|brand|string|Describes the brand of a product or offering.|Ford, Chevrolet, Dodge, Levis, Columbia, Patagonia|||||||
|isDisplayed|boolean|Helper node used by AA Product String Builder to set product scoped events|true|||||||
|itemPosition|integer|Integer position of a property within a sorted result. The first returned is position 1. For map results, this value can be the rank by distance from POI.|1, 2, 3, 4, 5||||0|||
|listingDriver|string|Describes the action that caused the listing to be displayed|Onsite Search, Curated Assortment, Navigation|||||||
|listingType|string|The type of results being listed|text, product, location, event, room, product location|||||||
|name|string|Name of the product or offering.  Should be unique and 1:1 with productID|Oceana, Corsica, Flame Tech, Air Jordan 88|||||||
|priceType|string|Describes the type of price offered using commonly used terms. |1st mark, 2nd mark, 3rd mark, clearance, sale, doorbuster|||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
|ratingAverage|string|String representation of the average customer rating.  Positive. Up to two decimal places. This is most often a number between 0 and 5. |1.1, 2, 5|^[0-9]*(\.[0-9]{1,2})?$||||||
|sku|string|Stock Keeping Unit (SKU) Unique Identifier of specific item (typically) held in inventory.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level below productID for products with SKU variants. |34567890, 4567890, 00155-large-cornflower|||||||
|status|string|Described the product's status|In Stock, Out of Stcok, Back-Ordered|||||||
