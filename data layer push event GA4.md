// Measure adding a product to a shopping cart by using an 'add' actionFieldObject
// and a list of productFieldObjects.
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({

{
  "event": "add_to_cart",
  "ecommerce": {
    "items": [
    {
      "item_id":'{{ID of the product}}',
                  "item_name": '{{Name of the product}}',
                  "item_category": '{{Category of the product}}',
                  "item_variant": '{{Variant of the product}}',
                  "price": '{{Price of the product}}',
                  ‘sale’: {{ sale item (maybe boolean for this)}}

      "quantity": {{ Quantity of the product}}
    }
    ]
  }
};
