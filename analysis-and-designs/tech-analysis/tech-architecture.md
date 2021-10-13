# Tech Architecture

![](<../../.gitbook/assets/tech architecture (1).jpg>)

The whole system in the Django-Rest will split into several sub-services, such as Admin Service, Customer Service, Catalog Service, Order Service, Product Service, and Shopping Cart Service. The detailed functions of each service are shown below.

| Service Name          | Functions                                                                                                                  | Connected DBs                                                                                        |
| --------------------- | -------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| Admin Service         | <p>Admin user login / register</p><p>Admin user management</p><p>...</p>                                                   | PostgreSQL                                                                                           |
| Customer Service      | <p>Customer user login / register</p><p>Customer user management</p><p>...</p>                                             | PostgreSQL                                                                                           |
| Catalog Service       | <p>Catalog management</p><p>...</p>                                                                                        | PostgreSQL                                                                                           |
| Order Service         | <p>Order creating</p><p>Order fulfillment</p><p>Order management</p><p>...</p>                                             | <p>MongoDB (for redundant product info)</p><p>PostgreSQL (ACID transaction)</p>                      |
| Product Service       | <p>Product management</p><p>Product publish / recover</p><p>Product searching</p><p>Product recommendation</p><p>...</p>   | <p>MongoDB (schema-less)</p><p>ES (product searching)</p><p>Neo4j (product recommendation)</p>       |
| Shopping Cart Service | <p>Shopping display</p><p>Add / Remove products</p><p>Change amounts of items</p><p>Submitting shopping cart</p><p>...</p> | <p>Redis (HA shopping cart)</p><p>RabbitMQ (asynchronous process)</p><p>PostgreSQL (persistence)</p> |
