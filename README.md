
# Vendor Management System Using DJANGO
Develop a vendor management system in Django with REST APIs using Django Rest Framework to showcase vendor performance and track purchase orders, securing every endpoint with JWT token authentication.

## Requirements
- Django (version 4.2.7)
- Python (version 3.10)

## Project Setup

```bash
python -m django startproject project_name
python manage.py startapp app_name

## Documentation

- After setting up the project, make sure to include the app_name in the INSTALLED_APPS list in the project's settings.py file.
- Then, connect the project's main URLs to the URLs of the app by including the app's URLs in the project's main URLs configuration.





## Database setup

After creating the models in Vendor (Vendor), Purchase_orders (PurchaseOrder), and Performance (VendorPerformance), make sure to register these models in their corresponding admin.py files.

Then run migrations in terminal
```bash
Python manage.py makemigrations
python manage.py migrate

## Run Server

Run server -  python manage.py runserver
## API Endpoints

VENDOR API
- POST    : api/vendors/post/
- GET     : api/vendors/get/
- GET(ID) : api/vendors/get/<int:vendor_id>
- PUT(ID) : api/vendors/put/<int:vendor_id>
- DELETE  : api/vendors/delete/<int:vendor_id>


PURCHASE_ORDER API

- POST    : api/purchase_orders/
- GET     : api/purchase_orders/
- GET(ID) : api/purchase_orders/<int:pk>/
- PUT(ID) : api/purchase_orders/<int:pk>/
- DELETE  : api/purchase_orders/<int:pk>/

VENDOR PERFORMANCE

- GET     : api/vendors/performance/