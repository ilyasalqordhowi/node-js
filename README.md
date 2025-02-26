| Parameter                            | Method         | Description                              |
| :----------------------------------- | :------------- | :--------------------------------------- |
| User registration and authentication |
| `/register`                          | `POST`         | `create a new account`                   |
| `/login`                             | `POST`         | `Log in as a registered account`         |
| Viewing and searching products       |
| `/products`                          | `GET`          | `get all products`                       |
| `/products`                          | `GET/search?=` | `get the product you want to search for` |
| Shopping cart                        |
| `/cart`                              | `POST`         | `Adding items to a shopping cart`        |
| `/cart`                              | `GET`          | `get items from the shopping cart`       |
| Checkout                             |
| `/checkout`                          | `POST`         | `Completing a purchase`                  |
