# Shoestore

## Description:
 <p>The project, created with React, is an e-commerce for shoes, in which the user can select different shoes that are divided by brand, add to the cart, check the product information, and finalize the purchase. The front-end was divided into several components that represent the site's elements, as well as contexts to store user information and the token needed to make requests. In the back-end, the code was created following a layered architecture, with routers, middleware and controllers. The bcrypt library was also used to encrypt the passwords of registered users.</p>

 ## Front-end
<p>Made using React.js</p>

* Login persistence check
* Access authenticated by token verification using uuid
* UseNavigate to change routes

## Back-end
<p>Made using Node.js, Express.js, and MongoDB</p>

* Using express Router to divide the backend layers into routers, middleware and controllers.
* Account creation with encrypted password using bcrypt
* Request validation in the backend using Joi

## Collections of MongoDB
The Database was divided by this manner:

### users
{<br/>
  name: string<br/>
  email: string<br/>
  password: string<br/>
  address: string<br/>
  phone: string<br/>
}<br/>
### sessions
{<br/>
  userId: number<br/>
  token: string<br/>
  lastStatus: Date<br/>
}<br/>
### items
{<br/>
  name: string<br/>
  price: number<br/>
  description: string<br/>
  type: string<br/>
  image: string<br/>
}<br/>
### carts
{<br/>
  userId: number<br/>
  cart: [ ]<br/>
}<br/>
### history
{<br/>
  userId: number<br/>
  name: string<br/>
  products: [ ]<br/>
  address: string<br/>
  fone: string<br/>
  email: string<br/>
  sum: number<br/>
}<br/>
