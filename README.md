# flask_api_design
Flask API Design - This is a sample library to refer to http call.

* api_db.py -- Basic GET call with database interaction (Database - SQLLite - books.db)

1. Home Page - http://127.0.0.1:5000/
2. GET request - http://127.0.0.1:5000/api/v1/resources/books?id=2

* api.py -- This is implementation from Miguel Grinberg's below blog.
https://blog.miguelgrinberg.com/post/designing-a-restful-api-with-python-and-flask

HTTP protocol - CRUD
==========================
POST    - Create
GET     - Read
PUT     - Update
DELETE  - Delete

* GET http://127.0.0.1:5000/todo/api/v1.0/tasks/fetchall
       - Fetches all records
* GET http://127.0.0.1:5000/todo/api/v1.0/tasks/1 
       - Fetches 1 record
* POST http://127.0.0.1:5000/todo/api/v1.0/tasks ; 
       - body : {"description": "Test Description", "title":"Read a book", "done":true}
       - Content-Type : "application/json"
       - This request creates a new record
* PUT http://127.0.0.1:5000/todo/api/v1.0/tasks/2     
       - body - {"done":true}
       - Update content of a record  
* DELETE http://127.0.0.1:5000/todo/api/v1.0/tasks/3  
       - Delete record 3 

For the dependencies, see requirements.txt
