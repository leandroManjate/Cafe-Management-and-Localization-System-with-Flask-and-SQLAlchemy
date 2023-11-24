# Cafe-Management-and-Localization-System-with-Flask-and-SQLAlchemy

### Description

This is a simple Flask API for finding cafes. Users can get details of cafes, such as name, location, seating capacity, facilities, and coffee price. The data is stored in a SQLite database, and the API supports operations like CREATE, READ, UPDATE, and DELETE (CRUD).

### Prerequisites

- Python 3.x
- pip or pip3
- Flask
- Flask-SQLAlchemy

### Installation

1. **Clone the repository.**
    ```
    git clone https://github.com/leandroManjate/Cafe-Management-and-Localization-System-with-Flask-and-SQLAlchemy.git
    ```
2. **Navigate to the project directory.**
    ```
    cd Cafe-Management-and-Localization-System-with-Flask-and-SQLAlchemy
    ```
3. **Install required packages.**
    ```bash
    # For Windows
    python -m pip install -r requirements.txt

    # For MacOS
    pip3 install -r requirements.txt
    ```

### Usage

1. **Run the application.**
    ```bash
    python main.py
    ```
2. **Open a web browser and go to `http://127.0.0.1:5000/` to see the homepage.**

### API Endpoints

- **GET `/random`**: Returns a random café.
- **GET `/all`**: Returns details of all cafes.
- **GET `/search?loc={location}`**: Search for cafes at a particular location.
- **POST `/add`**: Adds a new café.
- **PATCH `/update-price/{cafe_id}?new_price={new_price}`**: Updates the coffee price of a café with a specific ID.
- **DELETE `/report-closed/{cafe_id}`**: Deletes a café with a specific ID.

### Example Requests

1. **To get a random café:**
    ```http
    GET http://127.0.0.1:5000/random
    ```
2. **To add a new café:**
    ```http
    POST http://127.0.0.1:5000/add
    ```
    with form data like:
    ```plaintext
    name=Example Cafe
    map_url=http://map.example.com
    img_url=http://image.example.com
    loc=Example Location
    sockets=true
    toilet=true
    wifi=true
    calls=false
    seats=50
    coffee_price=£3.50
    ```

### Contributing

Feel free to submit issues and pull requests.

### License

This project is licensed under the MIT License.
I am editing the README file. Adding some more details about the project description.
