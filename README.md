| Parameter                            | Method | Description                              | Example                                   | Body                                          |
| :----------------------------------- | :----- | :--------------------------------------- | :---------------------------------------- | :-------------------------------------------- |
| User registration and authentication |
| `/register`                          | `POST` | `create a new account`                   | `http://localhost:8888/register `         | `id,username,email,password,confirm `password |
| `/login`                             | `POST` | `Log in as a registered account`         | `http://localhost:8888/login `            | `email,password   `                           |
| Viewing and searching products       |
| `/products`                          | `GET`  | `get all products`                       | `http://localhost:8888/products`          | `id,name,price,stock`                         |
| `/products`                          | `GET`  | `get the product you want to search for` | `http://localhost:8888/products?search= ` | `id,name`                                     |
| Shopping cart                        |
| `/cart`                              | `POST` | `Adding items to a shopping cart`        | `http://localhost:8888/cart`              | `id,productId,customerId`                     |
| `/cart`                              | `GET`  | `get items from the shopping cart`       | `http://localhost:8888/cart`              | `id,productId,customerId`                     |
| Checkout                             |
| `/checkout`                          | `POST` | `Completing a purchase`                  | `http://localhost:8888/checkout`          | `id,productId,customerId,order date`          |
