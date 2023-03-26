API Endpoint 

## Manipulating  clients API's:

- GET /clients - For retrieving all clients
- GET /client/{id} - For retrieving a specific client
- POST /client - For creating a new client
- PUT /client/{id} - For updating a client
- DELETE /client/{id} - For deleting a client

# Sample JSON data:

{
        "id": 1,
        "name": "Ak",
        "location": "pune",
        "start_date": "1-10-2010",
        "end_date": "20-11-2014"
    }

# Manipulating Projects API's:

- GET /projects - For retrieving all projects
- GET /projects/{id} - For retrieving a specific project
- POST /projects - For creating a new project
- PUT /projects/{id} - For updating a project
- DELETE /projects/{id} - For deleting a project

# Sample JSON data:
{
    "id": 2,
    "name": "c++",
    "owner_client": "Jayesh",
    "owner_consultant": "kiran",
    "start_date": "1-12-2010",
    "end_date": "11-3-2020",
    "status": "completed"
}
 

# Manipulating Employees API's:

- GET /employees - For retrieving all employees
- GET /employee/{id} - For retrieving a specific employee
- POST /employee - For creating a new employee
- PUT /employee/{id} - For updating a employee
- DELETE /employeee/{id} - For deleting a employee

 # Sample JSON data:

{
            "id": 1,
            "name": "Rakesh",
            "email": "Rakesh234@gmail.com",
            "contact": "7833335456545",
            "gender": "male",
            "dob": "01-12-2000",
            "designation": "developer",
            "address": "sangmner",
            "work_location": "pune",
            "date_of_joining": "12-12-2012",
            "date_of_exit": "01-12-2020",
            "manager": "vijay",
            "total_leaves": "1",
            "leave_balance": "4000"
        }

# Sample JSON data for inserting mapping relation within entities through projects

{
    "id": 2,
    "name": "c++",
    "owner_client": "Jayesh",
    "owner_consultant": "kiran",
    "start_date": "1-12-2010",
    "end_date": "11-3-2020",
    "status": "completed",
    "clientTable": {
        "id": 1,
        "name": "Ak",
        "location": "pune",
        "start_date": "1-10-2010",
        "end_date": "20-11-2014"
    },
    "employeeTable": [
        {
            "id": 1,
            "name": "Rakesh",
            "email": "Rakesh234@gmail.com",
            "contact": "7833335456545",
            "gender": "male",
            "dob": "01-12-2000",
            "designation": "developer",
            "address": "sangmner",
            "work_location": "pune",
            "date_of_joining": "12-12-2012",
            "date_of_exit": "01-12-2020",
            "manager": "vijay",
            "total_leaves": "1",
            "leave_balance": "4000"
        }
        
    ]

}

