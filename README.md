# # # BAN6420: Programming in R & Python
# Module 3
# Milestone Assignment 1
# Policy Management System for an Insurance Company

# Name: Babalola Taiwo
# Learner IS: 162894

  Description
  This code demonstrates how multiple classes ("Policyholder", "Product", and "Payment") create in seperate files
  interact to simulate a system for managing policyholders, products (insurance), and payments.
  
  1.  Create Class
        Below 3 class of module was create in seperate files
          -  Policyholder
              To create a policyholder, enroll them in a product, add a payment, and update their status as needed.
                      -    Handles managing policyholder information, including name, status, and the products they are enrolled in.
                      -    Allows registering, suspending, and reactivating a policyholder.
                      -    Manages enrolling in products and displaying account details.
          -  Product.py
              To manage product life cycles, from creation to removal and reactivation, and provides a way to update the details of products as needed.
                        -    Handles creating insurance products.
                        -    To manage the status of a product (active or inactive).
                        -    The "remove_product()" method deactivates the product.
          - Payment.py
               To manage policyholder accounts, processing payments, applying penalties, and handling product statuses accordingly.
                        -    Handles processing payments.
                        -    Associates payments with specific policyholders and products.
                        - Likely updates the policyholder’s balance when a payment is made.
  3. Import Statements from class files
       The import statements was used to bring in the classes "Policyholder", "Product", and "Payment" from class module files created in step 1.
       
  4. Product Management
       Three "Product" objects are created, each representing an insurance product:
            - "product1" is Health Insurance with a price of 150.
            - "product2" is Car Insurance with a price of 200.
            - "product3" is House Insurance with a price of 500.
            - The "Product" class is expected to accept an ID, name, and price for each product.
  5. Policyholder Class
       Three "Policyholder" objects are created, each representing a different person:
            - "Policyholder1" is Jark Clark with ID 401.
            - "Policyholder2" is Averi Kumar with ID 402.
            - "Policyholder3" is Rakesh Olye with ID 403.
            - The "Policyholder" class likely accepts an ID and name as arguments.

  6. Register Policyholders
            - The "register()" method of the "Policyholder" class will sets their status to "active" and indicates that they have been registered within the system.
            - This action is followed by a print statement (inside the "register()" method) that confirms their registration.

  7. Policyholders Enroll in Products
       The "add_product()" method of the "Policyholder" class is called for each policyholder, enrolling them in a product (insurance).
            - "policyholder1" is enrolled in "product1" (Health Insurance).
            - "policyholder2" is enrolled in "product2" (Car Insurance).
            - "policyholder3" is enrolled in "product3" (House Insurance).
            - The "add_product()" method checks if the product is active before enrolling the policyholder in it.

  8.   Process Payments
        Three "Payment" objects are created, one for each policyholder and product pair:
             -  "payment1" processes a payment of 150 for "policyholder1" and "product1" (Health Insurance).
             -  "payment2" processes a payment of 200 for "policyholder2" and "product2" (Car Insurance).
             -  Payment3" processes a payment of 500 for "policyholder3" and "product3" (House Insurance).
             -  The "process_payment()" method is called on each "Payment" object. This method likely marks the payment as successful,
                 dates the policyholder’s balance, or does other necessary actions.

  9.   Display Account Details
        This "display_account_details()" method of the "Policyholder" class is called for each policyholder.
        This is method likely prints out the policyholder's name, status, enrolled products, and payment history.
  
  10. Suspend Product and Policyholder
        The "remove_product()" method of the "Product" class is called on "product1". This likely marks the product (Health Insurance) as inactive or unavailable.
        The "suspend_policyholder()" method of the "Policyholder" class is called on "policyholder1", which likely changes their status to "suspended".

  11. Reactivate Product and Policyholder
        The status of "product1" is manually set to "'active'" (reactivating the Health Insurance product).
        The "reactivate_policyholder()" method of the "Policyholder" class is called on "policyholder1", reactivating the policyholder and changing their status back to "'active'".

  12. Suspend Another Policyholder
        Finally, the "suspend_policyholder()" method is called on "policyholder2" (Averi Kumar), changing their status to "'suspended'".
