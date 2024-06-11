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

![User-Register](https://github.com/Ansell10/Dressify-Login-Register/assets/128909158/26fd8150-e99d-4c23-9bfa-1ba3029be9b8)


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

![User-Login](https://github.com/Ansell10/Dressify-Login-Register/assets/128909158/5f04ef15-6261-4a77-a8b0-f3454b7ca9ff)


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

