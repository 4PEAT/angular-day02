### **Tasks for Product Management**

1. **Fetch and Display Products**
   - Fetch all products from the API using `getProducts()` in the `ProductService`.
   - Store the data in a `products` array in the `ProductsComponent`.
   - Display the products in a table using `*ngFor`.

2. **Add a New Product**
   - Create a form with fields for `Title`, `Price`, `Description`, `Image`, and `Category`.
   - Use `[(ngModel)]` to bind the form fields to a `newProduct` object in the `ProductsComponent`.
   - On form submission, call `addProduct()` to:
     - Send the new product to the API using `createProduct()` in `ProductService`.
     - Add the newly created product to the list.

3. **Edit an Existing Product**
   - Add an **Edit** button for each product in the table.
   - When clicked, populate an `editProduct` object with the selected product's data.
   - Display an edit form with the product details using `*ngIf="editProduct"`.
   - On form submission, call `updateProduct()` to:
     - Send the updated product to the API using `updateProduct()` in `ProductService`.
     - Update the product in the list.

4. **Delete a Product**
   - Add a **Delete** button for each product in the table.
   - When clicked, call `deleteProduct()` to:
     - Send a DELETE request to the API using `deleteProduct()` in `ProductService`.
     - Remove the deleted product from the list.

5. **Cancel Edit Mode**
   - Add a **Cancel** button in the edit form.
   - When clicked, reset the `editProduct` object to `null` to hide the form.
