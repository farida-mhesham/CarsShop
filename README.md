# Car Dealership Website

## Overview
The **Car Dealership Website** is a web application designed to showcase a collection of cars available for purchase or rent. It provides users with an intuitive interface to explore various car brands, view detailed car specifications, and contact the dealership. The platform also includes user authentication features for login and signup, enabling a personalized experience. Built with HTML, PHP, and JavaScript, this project aims to deliver a seamless and engaging user experience for car enthusiasts and potential buyers.

## Features
- **Homepage**: Displays featured cars, navigation links, and a contact section with business details.
- **Car Collection**: Showcases a variety of cars from multiple brands (Mitsubishi, BMW, Mercedes, Peugeot) with options to buy or rent.
- **Buy/Rent Page**: Provides detailed information about specific cars, including motor, horsepower, type, and drivetrain.
- **User Authentication**:
  - **Login**: Allows registered users to log in securely using email and password.
  - **Signup**: Enables new users to create an account.
- **Contact Section**: Includes dealership contact information (phone, address, business hours) and a form for inquiries.
- **Responsive Design**: Structured to be user-friendly across devices (though CSS styling is not included in the provided files).

## Project Structure
The project consists of the following files:
- `index.html`: The main homepage with featured cars, navigation, and contact information.
- `buy_rent.html`: A page for viewing car details and options to buy or rent.
- `car_collection_2.html`: Displays the full car collection organized by brand.
- `login.html`: User login page with a form for email and password.
- `signup.html`: User signup page for creating a new account.
- `login.php`: Backend script for handling user login with database connectivity.
- `script.js`: JavaScript file for client-side functionality (currently empty).

## Technologies Used
- **HTML**: For structuring the web pages.
- **PHP**: For server-side logic, including user authentication and database interaction.
- **JavaScript**: For client-side interactivity (to be implemented in `script.js`).
- **MySQL**: Database for storing user information (assumed based on `login.php`).
- **CSS**: Not provided but assumed for styling the HTML pages.

## Setup Instructions
### Prerequisites
- **Web Server**: Apache or any server supporting PHP (e.g., XAMPP, WAMP).
- **PHP**: Version 7.4 or higher.
- **MySQL**: For the user database.
- **Git**: For cloning the repository.

### Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/car-dealership-website.git
   cd car-dealership-website
   ```

2. **Set Up the Database**:
   - Create a MySQL database named `user_db`.
   - Create a `users` table with at least the following columns:
     ```sql
     CREATE TABLE users (
         id INT AUTO_INCREMENT PRIMARY KEY,
         email VARCHAR(255) NOT NULL UNIQUE,
         password VARCHAR(255) NOT NULL
     );
     ```
   - Update the database connection details in `login.php` if necessary (e.g., `$servername`, `$username`, `$password`, `$dbname`).

3. **Configure the Web Server**:
   - Place the project files in your web server's root directory (e.g., `htdocs` for XAMPP).
   - Ensure the server supports PHP and MySQL.

4. **Access the Application**:
   - Start your web server and MySQL service.
   - Open a browser and navigate to `http://localhost/car-dealership-website/index.html`.

## Usage
- **Homepage**: Navigate through the menu to explore new cars, the car collection, or contact the dealership.
- **Car Collection**: Browse cars by brand and view their prices with options to buy or rent.
- **Login/Signup**: Register a new account or log in to access personalized features.
- **Contact**: Use the contact form or provided details to reach out to the dealership.

## Future Improvements
- Add CSS styling for a polished and responsive design.
- Implement JavaScript functionality in `script.js` for interactive features (e.g., form validation, dynamic car filtering).
- Enhance security in `login.php` with additional input sanitization and error handling.
- Add a search feature to filter cars by brand, price, or type.
- Implement a backend for the contact form and buy/rent functionality.

## Contributing
Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit (`git commit -m "Add feature"`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.


## Contact
For questions or feedback, reach out via the contact form on the website or open an issue on GitHub.