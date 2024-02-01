## Backend API Endpoints for E-commerce Platform

### User Authentication
- `POST /auth/register`: Register a new user.
- `POST /auth/login`: Authenticate a user and return a token.
- `POST /auth/logout`: Log out a user and invalidate their token.
- `GET /auth/verify`: Verify a user's email address.
- `POST /auth/password-reset`: Request a password reset link.
- `POST /auth/password-update`: Update a user's password.

### User Management
- `GET /users/:id`: Retrieve a user's profile.
- `PUT /users/:id`: Update a user's profile.
- `DELETE /users/:id`: Delete a user's account.

### Product Management
- `GET /products`: List all products.
- `POST /products`: Create a new product.
- `GET /products/:id`: Retrieve a specific product.
- `PUT /products/:id`: Update a specific product.
- `DELETE /products/:id`: Delete a specific product.
- `GET /categories`: List all product categories.
- `POST /categories`: Create a new product category.
- `GET /categories/:id`: Retrieve a specific product category.
- `PUT /categories/:id`: Update a specific product category.
- `DELETE /categories/:id`: Delete a specific product category.

### Shopping Cart Functionality
- `GET /cart`: Retrieve the contents of the user's shopping cart.
- `POST /cart`: Add an item to the user's shopping cart.
- `PUT /cart/:itemId`: Update the quantity of an item in the user's shopping cart.
- `DELETE /cart/:itemId`: Remove an item from the user's shopping cart.
- `POST /cart/checkout`: Check out the items in the user's shopping cart.

### Order Processing
- `GET /orders`: List all orders for a user.
- `GET /orders/:id`: Retrieve a specific order.
- `POST /orders`: Create a new order.
- `PUT /orders/:id`: Update the status of a specific order.
- `DELETE /orders/:id`: Cancel a specific order.

### Payment Integration
- `POST /payments`: Process a payment for an order.
- `GET /payments/:id`: Retrieve the status of a payment.
- `POST /webhooks/payment`: Handle payment notifications from the payment gateway.

### Other Endpoints
- `GET /search`: Search for products.
- `GET /reviews`: List reviews for a product.
- `POST /reviews`: Submit a review for a product.
- `GET /shipping`: Get available shipping methods.
- `GET /shipping/:id`: Get details of a specific shipping method.

### Admin Endpoints
- `GET /admin/dashboard`: View admin dashboard statistics.
- `GET /admin/users`: List all users (for admins).
- `GET /admin/orders`: List all orders (for admins).
- `GET /admin/products`: Manage products (for admins).
- `GET /admin/categories`: Manage product categories (for admins).
- `GET /admin/payments`: Manage payments (for admins).
