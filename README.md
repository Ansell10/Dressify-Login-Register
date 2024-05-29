# Backend API for Register and Login (Dressify)

## Documentation
### Register
- URL
    - `/register`
- Method
    - `POST`
- Request Body
    - `email` as `string`, must be unique
    - `username` as `string`
    - `password` as `string`, must be at least 6 characthers
- Response
```json
{
    "error": false,
    "message": "User registered"
}
```

### Login
- URL
    - `/register`
- Method
    - `POST`
- Request Body
    - `email` as `string`, must be unique
    - `password` as `string`, must be at least 6 characthers
- Response
```json
{
    "error": false,
    "message": "Login successful",
    "loginResult": {
        "userId": "user-J0WEK5n55O0=",
        "email": "farhandp@gmail.com",
        "username": "testuser",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6InVzZXItSjBXRUs1bjU1TzA9IiwiaWF0IjoxNzE2NzI5NDMwLCJleHAiOjE3MTY3MzMwMzB9.ofbDhvUz_8K9pFdZoF-B-qTfooFzPhbAEUvkCcTX7j4"
    }
}
```

### Logout
- URL
    - `/logout`
- Method
    - `POST`
- Request Body
    - none
- Response
```json
{
    "error": false,
    "message": "Logout successful"
}
```

