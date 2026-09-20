# Database Documentation

## Main Collections / Tables

### Users

Stores customer and administrator information.

| Field    | Description            |
| -------- | ---------------------- |
| user_id  | Unique user identifier |
| name     | User name              |
| email    | User email             |
| password | Encrypted password     |
| role     | Customer or Admin      |

### Products

Stores product information.

| Field       | Description               |
| ----------- | ------------------------- |
| product_id  | Unique product identifier |
| name        | Product name              |
| description | Product description       |
| price       | Product price             |
| category_id | Product category          |
| quantity    | Available quantity        |

### Orders

Stores customer order information.

| Field        | Description             |
| ------------ | ----------------------- |
| order_id     | Unique order identifier |
| user_id      | Customer identifier     |
| order_date   | Date of order           |
| total_amount | Total order value       |
| status       | Current order status    |

### Payments

Stores payment-related information.

| Field          | Description               |
| -------------- | ------------------------- |
| payment_id     | Unique payment identifier |
| order_id       | Related order             |
| amount         | Payment amount            |
| payment_status | Payment status            |
| payment_date   | Date of payment           |

## Relationships

```text
User
 |
 | 1:N
 v
Orders
 |
 | 1:N
 v
Order Items
 |
 | N:1
 v
Products

Orders
 |
 | 1:1
 v
Payments
```
