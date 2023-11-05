## DB Design
<iframe style="border:none" width="800" height="450" src="https://whimsical.com/embed/BBxP7XU6xf9NtmaGdDF9eC"></iframe>

## API Design

1. Auth Service - NestJS - Rest
2. Restaurant Service - NestJS - GraphQL
3. User Service - NestJS - GraphQL
4. Delivery Service - NodeJS - GraphQL
5. Order Service - NodeJS - GraphQL
6. Communication Service - GoLang - Rest
7. Payment Service - NodeJS - Rest


## Auth Service
1. Register User - POST /api/v1/register
2. login User - POST /api/v1/login
3. Forget password - POST /api/v1/forget
4. verify OTP - POST /api/v1/verify

## User Service
1. Create User - POST /api/v1/users  => AuthId
2. Get User - GET /api/v1/users/:userId
3. Update User Details - PATCH /api/v1/users/:userId
4. List Users - GET /api/v1/users
   # Cart Service
5. CRUD on Products to Cart

## Restaurant Service
1. Create Restaurant - POST /api/v1/restaurants  => AuthId
2. Get Restaurant - GET /api/v1/restaurants/:restaurantId
3. Update Restaurant Details - PATCH /api/v1/restaurants/:restaurantId
   -- Menu:
   1. Create Menu - POST /api/v1/restaurants/:restaurantId/menu
   2. Create Item - POST /api/v1/restaurants/:restaurantId/menu/:menuId/item
   3. Get Menu - GET /api/v1/restaurants/:restaurantId/menu/:menuId
   4. Get Item - GET /api/v1/restaurants/:restaurantId/menu/:menuId/item/:itemId
   5. Update Menu - PATCH /api/v1/restaurants/:restaurantId/menu/:menuId
   6. Update Item - PATCH /api/v1/restaurants/:restaurantId/menu/:menuId/item/:itemId

   -- Features Related:
   1. Get All Items - GET /api/v1/restaurants/items
   2. Get All Menus - GET /api/v1/restaurants/menus

4. List Restaurants - GET /api/v1/restaurants


## Delivery Service
1. Create Delivery Boy - POST /api/v1/delivery  => AuthId
2. Get Delivery Boy - GET /api/v1/delivery/:deliveryId
3. Update Delivery Boy Details - PATCH /api/v1/delivery/:deliveryId
4. Check Driver Availability - GET /api/v1/delivery/:deliveryId/status


## Order:
1. Create Order - POST /api/v1/orders => RestaurantId, UserId, deliveryId
2. Get Order Status - GET /api/v1/orders/:orderId
3. Update Order - PATCH /api/v1/orders/:orderId
4. User Order History - GET /api/v1/users/:userId/orders
5. Restaurant Order History - GET /api/v1/restaurants/:restaurantId/orders
   
