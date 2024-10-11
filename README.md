
# Hero Management System

A Flask web application for managing heroes and their powers, built using SQLAlchemy for database interaction and Flask-Migrate for handling database migrations.

## Table of Contents

- [Features](#features)
- [Technologies](#technologies)
- [Installation](#installation)
- [Usage](#usage)
- [Models](#models)
- [Migrations](#migrations)
- [Contributing](#contributing)
- [License](#license)

## Features

- Manage a list of heroes and their associated powers.
- Use of SQLAlchemy for ORM and database interactions.
- Flask-Migrate for easy database migrations.
- Simple and intuitive RESTful API.

## Technologies

- **Flask**: A micro web framework for Python.
- **SQLAlchemy**: An ORM for database management.
- **Flask-Migrate**: Handles SQLAlchemy database migrations.
- **SQLite**: Lightweight database used for development.

## Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/Rickfalton/f4code1
   cd f4code1
   ```

2. **Running the Application**:

 ```bash
   code . 
   ```

3. **Install the required packages**:

   ```bash
   pipenv install
   pipenv shell
   ```


## Usage

1. **Run the application**:

   ```bash
   cd server
   python3 app.py
   ```

2. **Access the API**:

   Open your browser and navigate to `http://127.0.0.1:5000`.

## Models

### Hero

Represents a hero in the system.

- `id`: Unique identifier (Integer, Primary Key)
- `name`: Name of the hero (String)

### HeroPower

Represents a power associated with a hero.

- `id`: Unique identifier (Integer, Primary Key)
- `heroes_id`: Foreign key referencing `heroes.id` (Integer)
- `power`: Name of the power (String)

## Migrations

To create a new migration after modifying models, use:

```bash
flask db migrate -m "Description of changes"
flask db upgrade
```

## Contributing


1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```

