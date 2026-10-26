# Short Note — Olist Data Quality and ERD

In the customers table, `customer_id` identifies a record used to connect an order to its customer, whereas `customer_unique_id` groups records belonging to the same real customer, so the latter is more suitable for counting distinct customers. The `order_items` table acts as a junction between orders and products and also stores seller and item-level information. In the supplied data, every order row links to a customer, although a customer can have no orders. By contrast, some orders have no matching item rows, so the optional order-to-order_items relationship is supported by the observed data.

*Review these statements against your own query results before using this note.*
