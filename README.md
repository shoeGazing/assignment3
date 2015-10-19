# Assignment3

This is a continuation of [Assignment 2](https://github.com/erkartik91/assignment2). As a part of this assignment, you will focus on implementing a dynamic cart interface for the user.

## Tasks

1. **Add Price in product:** Modify your **product** and **cart** variables to include both the price and quantity now (earlier you had only the quantity). You can use following data format for the product and the cart. 
  ```
  var product = {
    'productName1' : {
      'price' : 10,
      'quantity' : 10
    },
    'productName2' : {
      'price' : 10,
      'quantity' : 10
    },
    ...
  };
  
  var cart = {
    'productName1' : 0,
    'productName2' : 0,
    ...
  };
  ```
  You **do not** need to keep price information in the cart as that information is already there in the products array. When calculcating the total price of the products in cart, you can use the price information from the products array. Please feel free to assign prices to products as you like.

2. **Cart Price / Timeout:** On the top right corner of your website, show a button with text **Cart ($0)**. Here $0 represent the total price for the products in the cart. For any product when the user clicks on **Add** button, the cart variable needs to be updated as well as the cart price shown should be updated as well. Use the products variable to calculate the total price of products in the cart. You also need to display the **inactiveTime** from previous assignment within the website footer. You can change the inactive time to 300s now. The footer should be updated every second to reflect the time user has been inactive.

3. **Hide Remove Button:** By default, when there is no product in the cart, when the user hovers over the product there should only be the **Add** button visible. **Remove** button for any product should only be visible when there is atleast one of that product in the cart.

4. **Show Cart:** When clicking on the  **Cart ($0)** button, the user should be presented with a Modal, that looks like [this](http://maxcdn.webappers.com/img/2011/03/css-modal.png). The modal should perform the following functionality
  - The modal should appear in the center of the window, with a transparent black bakground around the modal.
  - The modal should have a button to close the link in the top right corner, as shown in the link.
  - The model should present the user with the list of products in the cart, quantity of each product and total price and a tabular manner within the modal.
  - You also need to show **+/-** buttons in the table in the modal. Clicking on these buttons should increment/decrement the quantity of products in the cart. You can hook on to addToCart and removeFromCart functions, as they were already incrementing/decrementing the products in the cart.
  - If the quanity of the product reaches 0, you need to remove it completely from the tabular display in the modal.
  - The bottom of the modal should have a button called **Checkout**. Functionality for this button will be implemented in the next assignment.

## Bonus Task
When the cart modal is open, if the user presses **esc**, you need to hide the modal. This task is only counted if you are not using Bootstrap or any other framework. If you are using any of the frameworks, you can still implement this without using any of the frameworks deault modal functionality and get rewarded for this one.

## Submission instructions:

* Add a folder called **assignment3** in your github repo.
* Copy the code from your assignment2
* Update the code to reflect the changes for this assignment.
* Make sure you push your changes before midnight (11:59 PM) before the day when assignment is due - late submissions will not be accepted.
* We will be downloading the code on the midnight before the due date, any changes to code after that point will not be considered for marking.
