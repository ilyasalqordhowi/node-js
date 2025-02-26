| Parameter                            | Method | Description                              | Example                                   | Body                                                                                                                |
| :----------------------------------- | :----- | :--------------------------------------- | :---------------------------------------- | :------------------------------------------------------------------------------------------------------------------ |
| User registration and authentication |
| `/register`                          | `POST` | `create a new account`                   | `http://localhost:8888/register `         | `{"success":true,"message":success,"results":{ "id":1,"username":Ilyas,"email":ilyas@gmail.com,"phone":0888888 } }` |
| `/login`                             | `POST` | `Log in as a registered account`         | `http://localhost:8888/login `            | `{"success":true,"message":success,"results":{ "id":1,"username":Ilyass,"email":ilyas@gmail.com} }   `              |
| Viewing and searching products       |
| `/products`                          | `GET`  | `get all products`                       | `http://localhost:8888/products`          | `{"success":true,"message":success,"results":{ "id":1,"name":Iphone,price:200000,"stock":1 } }`                     |
| `/products`                          | `GET`  | `get the product you want to search for` | `http://localhost:8888/products?search= ` | `{"success":true,"message":success,"results":{ "id":1,"name":Iphone } }`                                            |
| Shopping cart                        |
| `/cart`                              | `POST` | `Adding items to a shopping cart`        | `http://localhost:8888/cart`              | `{"success":true,"message":success,"results":{ "id":1,"productId":1,"customerId":1 } }`                             |
| `/cart`                              | `GET`  | `get items from the shopping cart`       | `http://localhost:8888/cart`              | `{"success":true,"message":success,"results":{  "id":1,"productId":1,"customerId":1 } }`                            |
| Checkout                             |
| `/checkout`                          | `POST` | `Completing a purchase`                  | `http://localhost:8888/checkout`          | `{"success":true,"message":success,"results":{ "id":1,"productId":1,"customerId":1,"orderDate":26-2-2025 } }`       |
