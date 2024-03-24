Project Name- Shoppersstack
BaseURL- https://www.shoppersstack.com/shopping
Authorization-

Collection Shopper Profile

Request 1 - POST Register as a shopper /shoppers
  Raw Data - Required

  
Request 2 - POST Shopper Login /users/login
  Raw Data - Required

Requet 3 - GET Find Shopper data by shopperId /shoppers/{shopperId}
  Raw Data - Not Required
  
Request 4 -  PATCH Update the shopper Details /shoppers/{shopperId}
  Raw Data - Required

Request 5 - POST Genarates URL for forgot password /users/forgot-password
   Raw Data - Not required
     
Request 6 - POST Resets the password /users/reset-password
  Raw Data - 
  
Request 7 - POST Set user password /users/verify-account
  Raw Data - 

Collection Product View Action

Request 1 - GET Returns all the products /products
  Raw Data - Not Required

Request 2 - GET Returns all the default products /products/alpha
  Raw Data - Not Required

Collection Shopper Address

Request 1 - POST Add a new address /shoppers/{shopperId}/address
   Raw Data - Required
  
Request 2 - GET Get all the addresses /shoppers/{shopperId}/address
  Raw Data - Not required
   
Request 3 - GET Get a particular address by addressId /shoppers/{shopperId}/address/{addressId}
  Raw Ddata - Not Required
  
Request 4 - PUT Update an added address /shoppers/{shopperId}/address/{addressId}
  Raw Data - Required
  
Request 5 - DELETE Delete an address /shoppers/{shopperId}/address/{addressId}
  Raw Data - Not required

Collection Shopper Wishlist

Request 1 - POST Add a product to the wishlist /shoppers/{shopperId}/wishlist
  Raw Data - Required
  
Request 2 -  GET Get all the products from wishlist /shoppers/{shopperId}/wishlist
  Raw Data - Not Required

Request 3- DELETE Delete a product from wishlist /shoppers/{shopperId}/wishlist/{productId}
  Raw Data - Not Required
  
Collection Shopper Cart

Request 1 -POST Add a product to the cart /shoppers/{shopperId}/carts
Raw Data - Required

Request 2 -  GET Get all the products from the cart /shoppers/{shopperId}/carts
  Raw Data - Not Requrired

Request 3 - PUT Update a product in the cart /shoppers/{shopperId}/carts/{itemId}
  Raw Data - Required
  
Request 4- DELETE Delete a product from the cart /shoppers/{shopperId}/carts/{productId}
  Raw Data - Not Required

Collection Shopper Order

Request 1 - POST Place order from cart /shoppers/{shopperId}/orders
  Raw Data - Required
  
Request 2 - GET Display order history /shoppers/{shopperId}/orders
  Raw Data - Not Required

Request 3 - PATCH Update order status /shoppers/{shopperId}/orders/{orderId}
  Raw Data - Required
  
Request 4 - GET Generate Invoice copy /shoppers/{shopperId}/orders/{orderId}/invoice
  Raw Data - Not Required
  
Collection Shopper Product Review

Request 1 - POST Add a review to delivered product /reviews
  Raw Data - Required

Request 2 - GET Get all the reviews of a product  /reviews/{productId}
  Raw Data - Not Required

Request 3 - PUT Update an added review /reviews/{reviewId}
  Raw Data - Required
  
Request 4 - DELETE Delete an added review /reviews/{reviewId}
  Raw Data - Not Required
  
Collection Shopper Bank Cards

Request 1 - GET Creates the new card for a given bank /cards
  Raw Data - Not Required
  
Request 2 - PATCH Update card balance /cards
  Raw Data - Not required
  
Request 3 - POST Validates bank card with amount /cards/transaction
 Raw Data - Required
 
Request 4 - POST Validates bank card /cards/verify
  Raw Data - Required
  
Collection Shopper Profile Cards

Request 1 - POST Save the card data /cards
  Raw Data - Required

Request 2 - GET get the card data based on type /cards/{shopperId}
  Raw Data - Not required

Request 3 - GET Returns all the shoppers cards /shoppers/cards
  Raw Data - Not Required

Request 4 - DELETE Delete card data based on id /cards/{cardId}
  Raw Data - Not Required
  
Collection Shopper Bank Account

Request 1 - POST Create bank account /bankaccounts
Raw Data - Required

Request 2 - GET Get all bank account of shopper /bankaccounts
  Raw Data - Not required

Request 3 - PATCH Update bank account balance /bankaccounts
  Raw Data - Required
  
Request 4 - POST Validates bank account credential /bankaccounts/login
 Raw Data - Required

Collection Shopper Wallet Action

Request 1 - GET Get all Wallet Transactions /shoppers/{shopperId}/wallets
  Raw Data - Required

Collection Shopper Likes Action

Request 1 - GET Returns all the likes of shopper /shoppers/likes
  Raw Data - Not Required
  
Request 2 - DELETE Delete the shoppers like list /shoppers/likes
  Raw Data - Not Required
  
Request 3 - PATCH Update the shoppers like list /shoppers/likes
  Raw Data - Required
