# REST API to practies testing api using POSTMAN

# SERVER INFORMATION
```
Server: http://********:****
Token headder: using in all request
		Authorization: Token a27660c649afcaee39b94f7ece682cfb9649d4e7
```

# Get all items
```
Request:
url: /api/todos
method: GET

Response: return all item in json format
status code is 200 will be successful
Response body like that
[
    {
        "user": {
            "id": 1,
            "username": "admin",
            "email": "admin@gmail.com",
            "date_joined": "2018-04-05T03:46:43.227754Z"
        },
        "name": "study postman update task",
        "done": false,
        "date_created": "2018-04-05T03:48:21.899078Z"
    },
    {
        "user": {
            "id": 1,
            "username": "admin",
            "email": "admin@gmail.com",
            "date_joined": "2018-04-05T03:46:43.227754Z"
        },
        "name": "study postman update task",
        "done": true,
        "date_created": "2018-04-05T17:10:20.491359Z"
    },
    {
        "user": {
            "id": 1,
            "username": "admin",
            "email": "admin@gmail.com",
            "date_joined": "2018-04-05T03:46:43.227754Z"
        },
        "name": "study postman update task",
        "done": true,
        "date_created": "2018-04-05T17:10:27.978548Z"
    },
    {
        "user": {
            "id": 1,
            "username": "admin",
            "email": "admin@gmail.com",
            "date_joined": "2018-04-05T03:46:43.227754Z"
        },
        "name": "study postman update task",
        "done": true,
        "date_created": "2018-04-05T17:10:29.308474Z"
    },
    {
        "user": {
            "id": 1,
            "username": "admin",
            "email": "admin@gmail.com",
            "date_joined": "2018-04-05T03:46:43.227754Z"
        },
        "name": "study postman update task",
        "done": true,
        "date_created": "2018-04-05T17:10:30.581714Z"
    },
    {
        "user": {
            "id": 1,
            "username": "admin",
            "email": "admin@gmail.com",
            "date_joined": "2018-04-05T03:46:43.227754Z"
        },
        "name": "study postman update task",
        "done": true,
        "date_created": "2018-04-05T17:10:31.847959Z"
    }
]

```

# Get detail of todo item
```
# Request:
url: /api/todos/{{ todo_id }}
Method: GET

# Response: return a json that includes all atribute of item
status code is 200 will be successful
Response body like that:
{
    "user": {
        "id": 1,
        "username": "admin",
        "email": "admin@gmail.com",
        "date_joined": "2018-04-05T03:46:43.227754Z"
    },
    "name": "study postman update task",
    "done": false,
    "date_created": "2018-04-05T03:48:21.899078Z"
}

```

# Create a todolist
```
# Request:
url: /api/todos/
method: POST
BODY: you can change item attributes
{
    "user": {
        "id": 1,
        "username": "admin",
        "email": "sonlh@gmail.com",
        "date_joined": "2018-04-05T03:46:43.227754Z"
    },
    "name": "study postman update task",
    "done": false,
    "date_created": "2018-04-05T03:48:21.899078Z"
}

# Response: information of todo item which you have just created 
status code is 200 will be successful
Like that
{
    "user": {
        "id": 1,
        "username": "admin",
        "email": "sonlh@gmail.com",
        "date_joined": "2018-04-05T03:46:43.227754Z"
    },
    "name": "study postman update task",
    "done": false,
    "date_created": "2018-04-05T03:48:21.899078Z"
}
```

# Update a totolist
```
url: /api/todos/{{ todo_id }}
method: PUT
BODY: what you want to change. In my example I will change done atribute to true
{
    "user": {
        "id": 1,
        "username": "admin",
        "email": "sonlh@gmail.com",
        "date_joined": "2018-04-05T03:46:43.227754Z"
    },
    "name": "study postman update task",
    "done": true,
    "date_created": "2018-04-05T03:48:21.899078Z"
}

# Response: information of todo item which you have just updated
status code is 200 will be successful
Like that
{
    "user": {
        "id": 1,
        "username": "admin",
        "email": "sonlh@gmail.com",
        "date_joined": "2018-04-05T03:46:43.227754Z"
    },
    "name": "study postman update task",
    "done": true,
    "date_created": "2018-04-05T03:48:21.899078Z"
}
```

# Delete a toto item
```
# Request
url: /api/todos/{{ todo_id }}
method: DELETE

# Response: 
status code is 200 will be successful
status code is 404 means item is not existing
