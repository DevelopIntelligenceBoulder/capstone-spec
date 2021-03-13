# Project: Create an "Order Tracking" application
 
## Application Purpose
Amplify the productivity of TJX customer service representatives. You will create an application that allows CSRs to create and modify both customers and their orders, search a product catalog against which orders can be created, and manage the functional lifecycle of all orders.

## Tech Stack
* Backend 
    - (Express/Node.js) is required
    - The choice of additional Express middleware is unconstrained
* Frontend tech choices are left to your discretion
    - CSS: [Bulma](https://bulma.io/) is recommended 
    - JS: [JQuery](https://jquery.com/) is recommended
 
## Order Lifecycle
* Customer calls in an order
* CSR adds Customer if not existing
* CSR edits Customer as needed
* CSR Create an Order
* Add Product(s)
    - Check if available
    - Add if so
* CSR informs Shipping to assemble and ship the Order
* Shipping collects Products in Order
* Conditional at any point prior to shipping: Customer calls in to modify existing Order
* Order is shipped
* Order arrives
* Shipping agent informs CSR
* Order is closed

## Business Objects
* Orders
* Products
* Customers
* Users (CSRs)
 
## Application operations
### CSRs will be able to
* Authenticate themselves via a login mechanism
* CRUD for customer orders
* Browse the product catalog (as a CSR adds or removes products from an order, the product count needs to be updated)
* Browse the customer database
* Track the shipping status of the order (HOW DO WE WANT TO MODEL THEM CALLING AN EXTERNAL ASYNC API FOR UPDATES ON SHIPPING STATUS?)

## API starting point
 
## First steps
1. Discuss the architecture of the app amongst the team. Create a diagram that illustrates the flow data between various components.
2. Review the suggested API design and Business Object schemas. Do they support all of the functionality that is required for the application? Can you visualize which API methods will need to be called, and how the Business Objects will change at each step of the Order Lifecycle?
3. Encode the API using the OpenAPI specification. Doing so will not only serve as a canoncial source of living documentation, but also allow for the auto generation of client and server method stubs.
4. Review the suggested JS and CSS frameworks. Your choice of server side tech is non-negotiable in this case, but management defers to you regarding choice of front-end technologies.
5. ...
6. Profit!
 
 


