# Exercise
For this exercise, you will have to build a simple e-commerce shopping cart.

## Requirements
1. Implement a React application that shows information on the products and the shopping cart.
2. The following three components must be implemented:
   - `ProductList`: A component displaying a list of product cards. Use the appropriate CSS classes from the styles provided.
   - `ProductCard`: A component for an individual product card, displaying the caption and the price. It should have a button that can be clicked to add the product to the cart. (An item can be added multiple times)
   - `Cart`: A component that displays the number of items in cart, e.g. "6 items"
3. Use either Redux or React Context (and Reducer if necessary) to achieve state sharing among components.
4. 
## Provided Items

### Product List
A sample product list in the form of a JS array (_not_ JSON!) has been provided to you (you can assume the `id` field will always have unique values).

```javascript
const products = [
  { id: 1, caption: 'T-Shirt', price: 500 },
  { id: 2, caption: 'Shirt', price: 1000 },
  { id: 3, caption: 'Trousers', price: 1000 },
  { id: 4, caption: 'Jeans', price: 1500 },
  { id: 5, caption: 'Dress', price: 5500 },
  { id: 6, caption: 'Suit', price: 7500 }
]
```

### Styles

The CSS is provided for your convenience. It is up to you how you use these classes (feel free to rename the selectors if necessary).

```css
 body {
  background-color: #ddd;
  display: flex;
  justify-content: center;
 }

 #app {
  margin: 40px;
  max-width: 1600px;
  padding: 30px;
  background-color: #fff;
  color: #333;
  border-radius: 5px;
  position: relative;
 }

 .product-list {
  display: flex;
  flex-wrap: wrap;
 }

 .product {
  width: 120px;
  margin: 5px;
  padding: 20px;
  box-shadow: 0px 1px 4px #1113;
  text-align: center;
 }

 .product button {
  border: 0;
  background-color: #333;
  color: #fff;
  padding: 6px;
  width: 100%;
  text-transform: uppercase;
  cursor: pointer;
 }

 .product button:hover {
  background-color: #555;
 }

 .cart {
  position: absolute;
  top: 4px;
  right: 8px;
  font-size: smaller;
 }
```

## Notes
1. Looking up help online is okay, but full screen sharing must be on. Only static resources may be consulted. No help should be sought live, from another person online.
2. You can implement the solution in either JavaScript or TypeScript.
3. Some states are better passed as props, others might be better to put in the global state. Use your best judgment.
