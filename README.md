# E-commerce API Project

This project is part of a Python mini-course by Rocketseat. The goal is to build a simple e-commerce API using Flask, which simulates an online shopping system. Through this course, you'll learn how to create routes, integrate a database, implement user authentication, and provide essential functionalities like product listing, shopping cart management, and checkout.

## Project Structure

```plaintext
|- instance
|  |- ecommerce.db
|
|- app.py
|- requirements.txt
|- swagger.yaml
```

- **instance/**: Contains the SQLite database file (`ecommerce.db`) used by the application.
- **app.py**: The main application file where the API logic is implemented.
- **requirements.txt**: Lists all the dependencies required to run the project.
- **swagger.yaml**: Contains API documentation in the Swagger/OpenAPI format.

## Features

### User Authentication
- **Login**: Users can log in by providing their username and password. A session is created upon successful login.
- **Logout**: Users can log out to terminate their session.

### Product Management
- **Add Product**: Authenticated users can add new products to the store by providing a name, price, and optional description.
- **Update Product**: Authenticated users can update existing product details like name, price, and description.
- **Delete Product**: Authenticated users can delete products from the store.
- **Get Product Details**: Retrieve details of a specific product by its ID.
- **List Products**: View a list of all available products in the store.

### Shopping Cart
- **Add to Cart**: Authenticated users can add products to their shopping cart.
- **Remove from Cart**: Authenticated users can remove items from their shopping cart.
- **View Cart**: Authenticated users can view the contents of their shopping cart.
- **Checkout**: Authenticated users can check out, which clears the shopping cart after purchase.

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/ecommerce-api-flask.git
    cd ecommerce-api-flask
    ```

2. **Create a virtual environment**:
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

3. **Install the dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Set up the database**:
    ```bash
    flask db init
    flask db migrate
    flask db upgrade
    ```

5. **Run the application**:
    ```bash
    flask run
    ```

## API Documentation

The API endpoints and their descriptions can be found in the `swagger.yaml` file. You can use this file with Swagger UI to interact with and test the API.

## Database

This project uses SQLite as the database for simplicity. The database file (`ecommerce.db`) is located in the `instance/` folder.

## Dependencies

- **Flask**: Micro web framework for Python.
- **Flask-SQLAlchemy**: Adds SQLAlchemy support to Flask applications.
- **Flask-Login**: Provides user session management for Flask.
- **Flask-CORS**: Enables Cross-Origin Resource Sharing (CORS) in Flask.
- **SQLite**: A lightweight, disk-based database that doesn’t require a separate server process.

For a complete list of dependencies, see the `requirements.txt` file.

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue if you have suggestions for improvements.