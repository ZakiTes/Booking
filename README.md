# Hotel Booking Site

## Description

This project is a web-based hotel booking site developed using Node.js, Express.js, Sequelize ORM, and Passport for user authentication. It allows users to sign up, log in, browse a list of available hotels, view hotel details, make reservations for rooms, and rate hotels after their stay. The API documentation is provided using Swagger.

## Installation

1. **Clone this repository:**
   ```bash
   git clone <repository_url>
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Create a `.env` file in the root directory and configure environment variables:**
   ```dotenv
   PORT=3000
   DATABASE_NAME=your_database_name
   ADMIN_USERNAME=your_database_username
   ADMIN_PASSWORD=your_database_password
   HOST=your_database_host
   DIALECT=mysql
   DIALECTMODEL=your_dialect_model
   ```

## Usage

1. **Start the application:**
   ```bash
   npm start
   ```

2. **Access the application in your web browser at** `http://localhost:3000`.

3. **Explore the available endpoints and API documentation at** `http://localhost:3000/doc`.

## Endpoints

- **GET /**: Home page displaying a list of available hotels.
- **GET /login**: Login page for users to authenticate.
- **POST /login/password**: Endpoint to handle user login.
- **POST /logout**: Endpoint to handle user logout.
- **GET /signup**: Signup page for users to create an account.
- **POST /signup**: Endpoint to handle user signup.
- **GET /users/{userId}**: Retrieve user details by ID.
- **DELETE /users/{userId}**: Delete a user by ID.
- **GET /hotels/**: Retrieve a list of all available hotels.
- **POST /hotels/**: Create a new hotel.
- **DELETE /hotels/**: Delete a hotel.
- **GET /hotels/{hotelId}**: Retrieve hotel details by ID.
- **POST /hotels/{hotelId}/rate**: Post a rating for a hotel.
- **GET /rooms/{hotelId}**: Retrieve available rooms for a hotel.
- **GET /rooms/**: Retrieve a list of all available rooms.
- **POST /rooms/**: Create a new room.
- **DELETE /rooms/**: Delete a room.
- **POST /rooms/reservation**: Make a reservation for a room.

## User Authentication

User authentication is implemented using Passport middleware. Passport provides strategies for authenticating with different types of credentials, such as username/password, OAuth, etc. In this project, we're using the passport-local strategy for authenticating users with a username and password.

## Dependencies

- **connect-sqlite3**: SQLite3 session store for Express.js.
- **cookie-parser**: Middleware for parsing cookies.
- **debug**: Debugging utility.
- **dotenv**: Loads environment variables from a .env file.
- **ejs**: Embedded JavaScript templates for rendering views.
- **express**: Web application framework for Node.js.
- **express-openid-connect**: OpenID Connect middleware for Express.js.
- **express-session**: Session middleware for Express.js.
- **http-errors**: Utility to create HTTP errors.
- **morgan**: HTTP request logger middleware.
- **mysql**: MySQL client for Node.js.
- **mysql2**: MySQL client for Node.js with Promise support.
- **passport**: Authentication middleware for Node.js.
- **passport-local**: Passport strategy for authenticating with a username and password.
- **sequelize**: Promise-based Node.js ORM for MySQL, PostgreSQL, SQLite, and MSSQL.
- **sqlite3**: SQLite3 client for Node.js.
- **swagger-autogen**: Automatically generates Swagger documentation.
- **swagger-ui-express**: Swagger UI middleware for Express.js.

## Contributing

Contributions are welcome! Please feel free to open an issue or submit a pull request for any enhancements or bug fixes.

## License

This project is licensed under the MIT License.



