# E-COMMERCE

## screenshots

### Admin Dashboard

![Screenshot 2024-12-27 212300](https://github.com/user-attachments/assets/339d625a-ca31-48e2-aaaf-46892f429ae8)

### Customer Homepage
![Screenshot 2024-12-27 212249](https://github.com/user-attachments/assets/9a22bea9-2cca-4b84-8c09-1362ebbb3d59)

### Cart
![Screenshot 2024-12-27 212542](https://github.com/user-attachments/assets/353332b3-c9de-410b-99aa-5ca71ae6e36b)

### Track Orders
![Screenshot 2024-12-27 212313](https://github.com/user-attachments/assets/827034db-28b9-49f1-bad4-1352ee849480)

## FUNCTIONS

## Customer

- Customer can view/search products without login.
- Customer can also add/remove product to cart without login (if customer try to add same product in cart. It will add only one)
- When customer try to purchase product, then he/she must login to system.
- After creating account and login to system, he/she can place order.
- There is a payment page also (just for demo, DONT FILL YOUR CARD DETAILS THERE ,By the way, website do not save that details)
- If customer click on pay button, then their payment will be successful and their order will be placed.
- Customer can check their ordered details by clicking on orders button.
- Customer can see the order status (Pending, Confirmed, Delivered) for each order
- Customer can Download their order invoice for each order

## - Customer can send feedback to admin

### Admin

- First admin will login ( for username/password run following command in cmd )

```
py manage.py createsuperuser
```

- Give username, email, password and your admin account will be created.
- After login, there is a dashboard (attached in screenshot) where admin can see how many customer is registered, how many products are there for sale, how many orders placed.
- Admin can add/delete/view/edit the products.
- Admin can view/edit/delete customer details.
- Admin can view/delete orders.
- Admin can change status of order (order is pending, confirmed, out for delivery, delivered)

## - Admin can view the feedbacks sent by customers.

### Other Features

- customer places order and admin deleted that user(fraud detection), then their orders will automatically deleted
    
- suppose 1 customer places 4 products order and admin deleted 2 product from website, then that 2 product order will also be deleted and other 2 will be their
    
- If user click on purchase button without having products in their cart, then website will ask to add product in cart first.
    

## HOW TO RUN THIS PROJECT

- Install Python(3.7.6) (Dont Forget to Tick Add to Path while installing Python)
- Open Terminal and Execute Following Commands :

```
pip install django==3.0.5
pip install django-widget-tweaks
pip install xhtml2pdf
```

- Download This Project Zip Folder and Extract it
- Move to project folder in Terminal. Then run following Commands :

```
py manage.py makemigrations
py manage.py migrate
py manage.py runserver
```

- Now enter following URL in Your Browser Installed On Your Pc

```
http://127.0.0.1:8000/
```

## Drawbacks/Loop Holes

- When user edit their profile then he/she must login again because their username/password is updated in db.
- Popup of product is added to cart is shown when click on Ecommerce logo (soon i will fix it)

## Disclaimer

This project is developed for demo purpose and it's not supposed to be used in real application.
