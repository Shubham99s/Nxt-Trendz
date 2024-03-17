Rolled out an innovative e-commerce **Nxt Trendz** platform patterned after Amazon and Flipkart.

● Designed pages for Login, Products, Product details and Cart with React Router and React components.

● Ensured user security through JWT tokens, REST API calls, and local storage.

Technologies used: React JS, JS, CSS, Routing, REST API Calls, Local Storage, JWT Token, 
Authorization, Authentication

- User Login credentials

  ```text
   username: rahul
   password: rahul@2021
  ```


### Set Up Instructions

<details>
<summary>Click to view</summary>

- Download dependencies by running `npm install`
- Start up the app using `npm start`
</details>

### Completion Instructions

<details>
<summary>Functionality added</summary>
<br/>

The app must have the following functionalities

- When an unauthenticated user tries to access the **Cart** Route, then the page should be navigated to **Login** Route

- Following are the features to be implemented

  - When invalid credentials are provided in the login form and Login button is clicked, then the respective error message from the response should be displayed

  - When the username and password are provided correctly and Login button is clicked, then the page should navigate to Home Route
 
  - When an unauthenticated user tries to access the Home Route, Products Route or Cart Route, then the page should be redirected to the Login Route
  - When an authenticated user tries to access the Home Route, Products Route or Cart Route, then the page should be navigated to the respective route
  - When an authenticated user tries to access the Login Route, then the page should be redirected to the Home Route
  - When the Logout button is clicked, then the page should be navigated to the Login Route
  - Added Filters Group like Category, Rating, Sort By price in the product page Route and also added clear filter functionality

  - When an authenticated user tries to add the same product multiple times
    - The quantity of the product should be updated accordingly, and the count of the cart items in the header should be remained same
    - The total amount and number of items in the cart should be displayed in the **Cart** Route

  - In each cart item in the cart
      - When the plus icon is clicked, then the quantity of the product should be incremented by one
      - When the minus icon is clicked, then the quantity of the product should be decremented by one
      - When the quantity of the product is one and the minus icon is clicked, then the respective product should be removed from the cart
      - Based on the quantity of the product, the product price and the Cart Summary, i.e the total cost should be updated accordingly

  - When an authenticated user clicks on the remove button, cart item should be removed from the cart list

  - When an authenticated user clicks on the **Remove All** button, all the cart items should be removed from the cart and [Empty Cart View](https://assets.ccbp.in/frontend/content/react-js/nxt-trendz-cart-features-empty-cart-view.png) should be displayed

- The `CartContext` has an object as a value with the following properties
  - `cartList` - this key stores the cart items
  - `removeAllCartItems` - this method is used to remove all the cart items in the `cartList`
  - `addCartItem` - this method adds the cart item to the `cartList`
  - `removeCartItem` - this method removes the cart item from the `cartList`
  - `incrementCartItemQuantity` - this method increases the quantity of a product in the `cartList`
  - `decrementCartItemQuantity` - this method decreases the quantity of a product in the `cartList`

</details>
