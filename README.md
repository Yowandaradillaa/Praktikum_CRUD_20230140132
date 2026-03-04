# User API Specification

## 1. Create User

Endpoint:
POST /api/users

Request Body:
```json
{
  "name": "Yowanda",
  "age": 20
}
```

Response Success (200):
```json
{
  "id": "random string",
  "name": "Yowanda",
  "age": 20
}
```
![img.png](img.png)



---

## 2. Get All Users

Endpoint:
GET /api/users

Response Success (200):
```json
[
  {
    "id": "uuid-1",
    "name": "Yowanda",
    "age": 20
  },
  {
    "id": "uuid-2",
    "name": "Radilla",
    "age": 22
  }
]
```
![img_1.png](img_1.png)

---

---

## 3. Update User

Endpoint:
PUT /api/users/{id}

Request Body:
```json
{
  "name": "Yowanda Updated",
  "age": 21
}
```

Response Success (200):
```json
{
  "id": "uuid-1",
  "name": "Yowanda Updated",
  "age": 21
}
```
![img_2.png](img_2.png)

---

## 5. Delete User

Endpoint:
DELETE /api/users/{id}

Example:
DELETE /api/users/uuid-1

Response Success (200):
```json
{
  "message": "user deleted successfully"
}
```
![img_3.png](img_3.png)

##Web Simple
![img_5.png](img_5.png)

##Database
![img_4.png](img_4.png)