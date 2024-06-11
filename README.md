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


### List
- URL
    - `/list`
- Method
    - `GET`
- Request Parameters 
    - `page` (optional, integer): Page number for pagination. Defaults to 1 if not provided.
    - `size` (optional, integer): Number of items per page. Defaults to 10 if not provided.
- Response
```json
{
    "error": false,
    "message": "Clothing items fetched successfully",
    "totalItems": 310,
    "totalPages": 31,
    "currentPage": 1,
    "pageSize": 10,
    "clothingItems": [
        {
            "id": 1,
            "gender": "Female",
            "type_of_clothing": "Tshirts",
            "color": "Black",
            "season": "Summer",
            "usages": "Casual",
            "product_display_name": "Nope Women Black T-Shirts",
            "picture_link": "https://storage.googleapis.com/clothing-dressify/data/1.png\r"
        },
        {
            "id": 2,
            "gender": "Female",
            "type_of_clothing": "Tshirts",
            "color": "Black",
            "season": "Rainy",
            "usages": "Casual",
            "product_display_name": "Knitwear Women Black T-Shirts ",
            "picture_link": "https://storage.googleapis.com/clothing-dressify/data/2.png\r"
        },
        {
            "id": 3,
            "gender": "Female",
            "type_of_clothing": "Tshirts",
            "color": "Black",
            "season": "Summer",
            "usages": "Casual",
            "product_display_name": "Black Butterfly Women T-Shirts",
            "picture_link": "https://storage.googleapis.com/clothing-dressify/data/3.png\r"
        },
        {
            "id": 4,
            "gender": "Female",
            "type_of_clothing": "Tshirts",
            "color": "White",
            "season": "Summer",
            "usages": "Casual",
            "product_display_name": "Cherry White Pink T-Shirts",
            "picture_link": "https://storage.googleapis.com/clothing-dressify/data/4.png\r"
        },
        {
            "id": 5,
            "gender": "Female",
            "type_of_clothing": "Tshirts",
            "color": "White",
            "season": "Summer",
            "usages": "Casual",
            "product_display_name": "Cute Dog Women T-Shirts",
            "picture_link": "https://storage.googleapis.com/clothing-dressify/data/5.png\r"
        },
        {
            "id": 6,
            "gender": "Female",
            "type_of_clothing": "Tshirts",
            "color": "White",
            "season": "Rainy",
            "usages": "Casual",
            "product_display_name": "Knitwear Women White T-Shirts ",
            "picture_link": "https://storage.googleapis.com/clothing-dressify/data/6.png\r"
        },
        {
            "id": 7,
            "gender": "Female",
            "type_of_clothing": "Tshirts",
            "color": "Blue",
            "season": "Rainy",
            "usages": "Casual",
            "product_display_name": "Blue Sweater Ocean",
            "picture_link": "https://storage.googleapis.com/clothing-dressify/data/7.png\r"
        },
        {
            "id": 8,
            "gender": "Female",
            "type_of_clothing": "Tshirts",
            "color": "Blue",
            "season": "Summer",
            "usages": "Casual",
            "product_display_name": "Croptop Women Blue T-Shirts",
            "picture_link": "https://storage.googleapis.com/clothing-dressify/data/8.png\r"
        },
        {
            "id": 9,
            "gender": "Female",
            "type_of_clothing": "Tshirts",
            "color": "Blue",
            "season": "Summer",
            "usages": "Sports",
            "product_display_name": "Sports Women Blue T-Shirts",
            "picture_link": "https://storage.googleapis.com/clothing-dressify/data/9.png\r"
        },
        {
            "id": 10,
            "gender": "Female",
            "type_of_clothing": "Tshirts",
            "color": "Brown",
            "season": "Summer",
            "usages": "Casual",
            "product_display_name": "Off-White Women Brown T-Shirts",
            "picture_link": "https://storage.googleapis.com/clothing-dressify/data/10.png\r"
        }
    ]
}


