# config-repository

Banking Manager APIs -

All Requests going to API - Gateway
-----------
USER Microservice APIs - 

GET ALL USERS
```bash
URL : http://localhost:9002/user/all-users
HTTP Method : GET
```
Json Response :
```json
[
    {
        "userId": 1311,
        "name": "Vaibhav Shrivastava",
        "email": "innomightmail@gmail.com",
        "phoneNumber": 9755057765,
        "account": {
            "accNo": 1001,
            "branch": "Jabalpur",
            "accountBalance": 9500,
            "userId": 1311,
            "ifsc": "ICIC098764"
        }
    },
    {
        "userId": 1312,
        "name": "Varun Shrivastava",
        "email": "varun@gmail.com",
        "phoneNumber": 9960543885,
        "account": {
            "accNo": 1002,
            "branch": "Jabalpur",
            "accountBalance": 8700,
            "userId": 1312,
            "ifsc": "ICIC056782"
        }
    },
    {
        "userId": 1313,
        "name": "Rajesh Shrivastava",
        "email": "rajesh@gmail.com",
        "phoneNumber": 7999459656,
        "account": {
            "accNo": 1003,
            "branch": "Jabalpur",
            "accountBalance": 8900,
            "userId": 1313,
            "ifsc": "ICIC017843"
        }
    }
]
```

GET USER
```bash
URL : http://localhost:9002/user/1311
HTTP Method : GET
```

Json Response :
```json
{
    "userId": 1311,
    "name": "Vaibhav Shrivastava",
    "email": "innomightmail@gmail.com",
    "phoneNumber": 9755057765,
    "account": {
        "accNo": 1001,
        "branch": "Jabalpur",
        "accountBalance": 9500,
        "userId": 1311,
        "ifsc": "ICIC098764"
    }
}
```

ADD USER
```bash
URL : http://localhost:9002/user/add-user
HTTP Method : POST
```
Json Request :
```json
{
    "name": "Kavita Shrivasta",
    "email": "kavita@gmail.com",
    "phoneNumber": "9827442418"
}
```
Json Response :
```json
{
    "userId": 9404,
    "name": "Kavita Shrivasta",
    "email": "kavita@gmail.com",
    "phoneNumber": 9827442418,
    "account": {
        "accNo": 8501,
        "branch": "Jabalpur",
        "accountBalance": 0,
        "userId": 9404,
        "ifsc": "ICIC152087"
    }
}

```

UPDATE USER
```bash
URL : http://localhost:9002/user/update-user
HTTP Method : POST
```
Json Request :
```json
{
    "userId": 9404
    "user": {
        "name": "Kavita Shrivasta Updated",
        "email": "kavita@gmail.com",
        "phoneNumber": "9827442418"
        }
}
```
Json Response :
```json
{
    "userId": 9404,
    "name": "Kavita Shrivasta Updated",
    "email": "kavita@gmail.com",
    "phoneNumber": 9827442418,
    "account": {
        "accNo": 8501,
        "branch": "Jabalpur",
        "accountBalance": 0,
        "userId": 9404,
        "ifsc": "ICIC152087"
    }
}

```



