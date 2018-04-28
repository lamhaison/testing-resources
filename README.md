# REST API to practies testing api using POSTNAME

# SERVER INFORMATION
```
Server: http://log.uiza.io:8091
Token headder:
		Authorization: Token a27660c649afcaee39b94f7ece682cfb9649d4e7
```

# Get all items
```
Request:
url: /api/todos
method: get

Response: status code is 200 will be successful
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
