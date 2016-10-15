# Assignment3

This is a continuation of [Assignment 2](https://github.com/shoeGazing/assignment2). As a part of this assignment, you will focus on implementing a dynamic cart interface for the user.

## Tasks

1. **Add Price in product:** (3 points) Modify your **product** and **cart** variables to include both the price and quantity now (earlier you had only the quantity). You can use following data format for the product and the cart. 
  ```
  var product = {
    'productName1' : {
      'price' : 10,
      'quantity' : 5
    },
    'productName2' : {
      'price' : 10,
      'quantity' : 5
    },
    ...
  };
  
  var cart = {
    'productName1' : 1,
    'productName2' : 3,
    ...
  };
  ```
  You **do not** need to keep price information in the cart as that information is already there in the products array. When calculating the total price of the products in cart, you can use the price information from the products array. Please feel free to assign prices to products as you like.

2. **Cart Price / Timeout:** (3 points) On the top right corner of your website, show a button with text **Cart ($0)**. Here $0 represent the total price for the products in the cart. For any product when the user clicks on **Add** button, the cart variable needs to be updated as well as the cart price shown should be updated as well. Use the products variable to calculate the total price of products in the cart. You also need to display the **inactiveTime** from previous assignment within the website footer. You can change the inactive time to 300s now. The footer should be updated every second to reflect the time user has been inactive.

3. **Hide Remove Button:** (2 points) By default, when there is no product in the cart, when the user hovers over the product there should only be the **Add** button visible. **Remove** button for any product should only be visible when there is at least one of that product in the cart. If a product is out of stock, display a friendly message to the user to indicate that the item is out of stock.

4. **Show Cart:** (4 points) When clicking on the  **Cart ($0)** button, the user should be presented with a Modal, that looks like [this](http://maxcdn.webappers.com/img/2011/03/css-modal.png). The modal should perform the following functionality
  - The modal should appear in the center of the window, with a transparent black background around the modal.
  - The modal should have a button to close the link in the top right corner, as shown in the link.
  - The model should present the user with the list of products in the cart, quantity of each product and total price and a tabular manner within the modal.
  - You also need to show **+/-** buttons in the table in the modal. Clicking on these buttons should increment/decrement the quantity of products in the cart. You can hook on to addToCart and removeFromCart functions, as they were already incrementing/decrementing the products in the cart.
  - If the quantity of the product reaches 0, you need to remove it completely from the tabular display in the modal.
  - The bottom of the modal should have a button called **Checkout**. Functionality for this button will be implemented in the next assignment.

## Bonus Task

(1 point) When the cart modal is open, if the user presses **esc**, you need to hide the modal. This task is only counted if you are not using Bootstrap or any other framework. If you are using any of the frameworks, you can still implement this without using any of the frameworks default modal functionality and receive credit for this task.

## Code Quality

(3 points) You should ensure that your JavaScript code follows the best practices around variable naming, variable placement, modularization (dividing long code blocks into smaller functions) and comments (at the minimum, describing what each function does). Your code will be assessed for code quality during marking.

## Scalability

(3 points)
There are multiple ways to go about implementing the tasks specified in this assignment. However, you should consider the scalability/robustness of your implementation. As an example, you should consider creating DOM elements programmatically (from Assignment 2 onwards) rather than hardcoding them in your HTML. Software designs that lead to "copy and paste programming" will be discouraged.

## Submission instructions:

* Copy the code from your assignment 2
* Update the code to reflect the changes for this assignment.
* Create a branch called assignment-3.
* Make sure you push your changes before the due date - late submissions will not be accepted.
* For students in L1A, the assignment is due on Monday, October 31 at 11:59 PM.
* For students in L1B, the assignment is due on Wednesday, November 2 at 11:59 PM.  
* We will be downloading the code on the due date, any changes to the code after that point will not be considered for marking.

## Labs are mandatory on the week of assignment submission:

* If you can not attend the lab to demo your assignment for any reason, you need to notify Instructors on Piazza at least 24 hours prior to the start of your lab section. Otherwise, you will be recorded as no attendance and will have marks deducted.
