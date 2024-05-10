## API Docs
1. User Authentication and Authorization:
   - `/api/auth/login` - POST: User login
   - `/api/auth/logout` - POST: User logout
   - `/api/auth/register` - POST: User registration
   - `/api/auth/reset-password` - POST: Reset user password

2. User Profile Management:
   - `/api/user/profile` - GET: Get user profile
   - `/api/user/profile` - PUT: Update user profile
   - `/api/user/profile/avatar` - PUT: Update user avatar
   - `/api/user/profile/address` - GET: Get user address
   - `/api/user/profile/address` - PUT: Update user address
   - `/api/user/profile/orders` - GET: Get user orders
   - `/api/user/profile/orders/:orderId` - GET: Get specific user order

3. Product Management:
   - `/api/products` - GET: Get all products
   - `/api/products/:productId` - GET: Get specific product
   - `/api/products/search` - GET: Search products
   - `/api/products/categories` - GET: Get all categories
   - `/api/products/categories/:categoryId` - GET: Get specific category and its products

4. Cart and Checkout:
   - `/api/cart` - GET: Get user's shopping cart
   - `/api/cart` - POST: Add item to cart
   - `/api/cart/:itemId` - PUT: Update item quantity in cart
   - `/api/cart/:itemId` - DELETE: Remove item from cart
   - `/api/checkout` - POST: Initiate checkout process
   - `/api/checkout/:orderId` - PUT: Update order information
   - `/api/checkout/:orderId/confirm` - POST: Confirm order

5. Order Management:
   - `/api/orders` - GET: Get all orders
   - `/api/orders/:orderId` - GET: Get specific order details
   - `/api/orders/:orderId/cancel` - PUT: Cancel order
   - `/api/orders/:orderId/track` - GET: Track order shipment

6. Seller Dashboard:
   - `/api/seller/dashboard` - GET: Get seller dashboard statistics
   - `/api/seller/products` - GET: Get seller's products
   - `/api/seller/products/:productId` - GET: Get specific product listed by seller
   - `/api/seller/products/:productId` - PUT: Update product details
   - `/api/seller/products/:productId` - DELETE: Remove product listing

7. Feedback and Reviews:
   - `/api/products/:productId/reviews` - GET: Get product reviews
   - `/api/products/:productId/reviews` - POST: Add review for product
   - `/api/orders/:orderId/review` - POST: Add review for order

8. Messaging:
   - `/api/messages` - GET: Get user's messages
   - `/api/messages/:messageId` - GET: Get specific message
   - `/api/messages/:userId` - POST: Send message to user

