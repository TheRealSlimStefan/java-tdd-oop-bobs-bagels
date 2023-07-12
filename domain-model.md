| Class    | Members                              | Methods                                        | Scenario                                           | Outputs |
|----------|--------------------------------------|------------------------------------------------|----------------------------------------------------|---------|
| `Basket` | `HashMap<Product, Integer> products` | `addProduct(Product product, int quantity)`    | Product is not in the basket and quantity is valid | true    |
|          | `basketCapacity`                     |                                                | Product is in the basket and quantity is valid     | true    |
|          | `basketQuantity`                     |                                                | quantity is not valid                              | false   |
|          |                                      |                                                | if basket is full                                  | false   |
|          |                                      | `removeProduct(Product product, int quantity)` | Product is in the basket and quantity is valid     | true    |
|          |                                      |                                                | Product is in not the basket and quantity is valid | false   |
|          |                                      |                                                | quantity is not valid                              | false   |
|          |                                      | `changeBasketCapacity(int newCapacity)`        | new capacity is valid                              | true    |
|          |                                      |                                                | new capacity is not valid                          | false   |
|          |                                      | `getTotalCost()`                               | returns total cost                                 | float   |

| Class     | Members   | Methods       | Scenario                | Outputs |
|-----------|-----------|---------------|-------------------------|---------|
| `Product` | `sku`     | `getPrice()`  | returns product's price | float   |
|           | `price`   |               |                         |         |
|           | `name`    |               |                         |         |
|           | `variant` |               |                         |         |