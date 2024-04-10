# Little Lemon Web Application
(Meta Back-End Developer Capstone Project)

## Django web application for a restaurant named Little Lemon
- Serves static HTML content using the Django framework
- Connects the backend to a MySQL database
- Implements APIs for menu and table booking
- Set up with user registration and authentication
- Contains unit tests
- The API can be tested with the Insomnia REST client

## API endpoints to test
| Description           | Method | Path                        | Token                                    | Form/JSON payload                                                         |
|-----------------------|--------|-----------------------------|------------------------------------------|---------------------------------------------------------------------------|
| Load static home page | GET    | /restaurant ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎                 |                                          |                                                                           |
| View menu items       | GET    | /restaurant/menu             ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎| 7cfa4c477a8dbea1b8df7a720a494bebe762d142 |                                                                           |
| View single menu item | GET    | /restaurant/menu/<<int:pk>>  ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎| 7cfa4c477a8dbea1b8df7a720a494bebe762d142 |                                                                           |
| Add a menu item       | POST   | /restaurant/menu ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎            | 7cfa4c477a8dbea1b8df7a720a494bebe762d142 | { "title": "Burger", "price": "4.00", "inventory": 10 }              |
| Update a menu item    | PUT    | /restaurant/menu/<<int:pk>> ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ | 7cfa4c477a8dbea1b8df7a720a494bebe762d142 | { "id": 2,	"title": "Spaghetti Bolognese",	"price": "7.00",	"inventory": 20 } |
| Delete a menu item    | DELETE | /restaurant/menu/<<int:pk>> ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ | 7cfa4c477a8dbea1b8df7a720a494bebe762d142 |                                                                           |
| Obtain authtoken      | POST   | /restaurant/api-token-auth ‎ ‎ ‎ ‎ ‎ ‎  ‎ ‎ ‎ ‎ ‎ ‎ |                                          | { "username": "testuser",	"password": "loremipsum" }                       |
| View table bookings   | GET    | /restaurant/booking/tables ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎ ‎  | 7cfa4c477a8dbea1b8df7a720a494bebe762d142 |                                                                           |
