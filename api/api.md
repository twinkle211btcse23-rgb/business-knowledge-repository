# API Documentation

## User APIs

### Register User

```text
POST /api/users/register
```

Creates a new user account.

### Login

```text
POST /api/users/login
```

Authenticates an existing user.

---

## Product APIs

### Get Products

```text
GET /api/products
```

Returns a list of available products.

### Get Product

```text
GET /api/products/:id
```

Returns details of a specific product.

### Add Product

```text
POST /api/products
```

Adds a new product to the system.

### Update Product

```text
PUT /api/products/:id
```

Updates an existing product.

### Delete Product

```text
DELETE /api/products/:id
```

Deletes a product.

---

## Order APIs

### Create Order

```text
POST /api/orders
```

Creates a new customer order.

### Get Orders

```text
GET /api/orders
```

Returns customer order information.

### Update Order Status

```text
PUT /api/orders/:id/status
```

Updates the status of an order.
