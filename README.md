Food Delivery API (FastAPI Project)

Overview

This project is a FastAPI-based Food Delivery Backend System that provides APIs for managing menu items, placing orders, handling cart operations, and performing advanced operations like filtering, searching, sorting, and pagination.

The system simulates a real-world food delivery workflow with structured endpoints and validation using Pydantic.


Features

Menu Management

* View all menu items
* Get item by ID
* Add new menu items
* Update menu items
* Delete menu items
* Menu summary (available/unavailable items)
* Filter menu (category, price, availability)
* Search menu (name/category)
* Sort menu (price, name, category)
* Pagination support
* Combined browse (filter + sort + pagination)



Cart System

* Add items to cart
* Update quantity if item already exists
* View cart with total price
* Remove items from cart
* Checkout cart (converts cart items into orders)


Order Management

* Place order directly
* View all orders
* Search orders by customer name
* Sort orders by total price
* Supports delivery and pickup orders

Technologies Used

* Python
* FastAPI
* Uvicorn
* Pydantic

 Project Structure

food_delivery_app/
│
├── main.py
├── requirements.txt
├── screenshots/
│   ├── Q1_home.png
│   ├── Q2_menu.png
│   └── ...
│
└── README.md

How to Run the Project
Step 1: Install dependencies

pip install -r requirements.txt

Step 2: Run the server

uvicorn main:app --reload
Step 3: Open Swagger UI

http://127.0.0.1:8000/docs

 API Endpoints
 Menu APIs

* GET /menu
* GET /menu/summary
* GET /menu/filter
* GET /menu/search
* GET /menu/sort
* GET /menu/page
* GET /menu/browse
* GET /menu/{item_id}
* POST /menu
* PUT /menu/{item_id}
* DELETE /menu/{item_id}

Order APIs

* GET /orders
* POST /orders
* GET /orders/search
* GET /orders/sort

 Cart APIs

* POST /cart/add
* GET /cart
* DELETE /cart/{item_id}
* POST /cart/checkout

 Testing

All APIs are tested using Swagger UI.

Screenshots for each question are included in the `screenshots/` folder as required.

Key Concepts Implemented

* REST API Design
* Pydantic Validation
* Query Parameters
* CRUD Operations
* Filtering, Searching, Sorting
* Pagination
* Data Handling using Lists
* Route Ordering in FastAPI
* Error Handling

Screenshots

All required screenshots are provided in the `screenshots/` folder, including API responses, validation errors, cart operations, and advanced query features.

Conclusion

This project demonstrates a complete backend system for a food delivery application using FastAPI. It covers essential backend development concepts and provides a scalable structure for future enhancements.

Author

Charan Kumar Reddy

