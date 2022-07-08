# UA DL push example
<script>
// Send transaction data with a pageview if available
// when the page loads. Otherwise, use an event when the transaction
// data becomes available.
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  'event': 'purchase', 
  'ecommerce': {
    'purchase': {
      'actionField': {
        'id': 'T12345',                         // Transaction ID.
        'affiliation': 'Online Store',
        'revenue': '35.43',                     // Total transaction value
        'tax':'4.90',
        'shipping': '5.99',
        'coupon': 'SUMMER_SALE'
      },
      'products': [{                            // List of productFieldObjects.
        'name': 'Triblend Android T-Shirt',     // Name or ID is required.
        'id': '12345',
        'price': '15.25',
        'brand': 'Google',
        'category': 'Apparel',
        'variant': 'Gray',
        'quantity': 1,
        'coupon': ''                            // Optional fields
       },
       {
        'name': 'Donut Friday Scented T-Shirt',
        'id': '67890',
        'price': '33.75',
        'brand': 'Google',
        'category': 'Apparel',
        'variant': 'Black',
        'quantity': 1
       }]
    }
  }
});
</script> 


# GA4 DL push example
<script>
dataLayer.push({
  "event": "purchase",
  "ecommerce": {
      "transaction_id": "T_12345",
      "affiliation": "Google Merchandise Store",
      "value": 25.42,
      "tax": 4.90,
      "shipping": 5.99,
      "currency": "USD",
      "coupon": "SUMMER_SALE",
      "items": [
       {
        "item_id": "SKU_12345",
        "item_name": "Stan and Friends Tee",
        "coupon": "SUMMER_FUN",
        "currency": "USD",
        "discount": 2.22,
        "item_brand": "Google",
        "item_category": "Apparel",
        "item_variant": "green",
        "price": 9.99,
        "quantity": 1
      },
      {
        "item_id": "SKU_12346",
        "item_name": "Google Grey Women's Tee",
        "coupon": "SUMMER_FUN",
        "currency": "USD",
        "discount": 3.33,
        "item_brand": "Google",
        "item_category": "Apparel",
        "item_variant": "gray",
        "price": 20.99,
        "quantity": 1
      }]
  }
}
});
</script>


