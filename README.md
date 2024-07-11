# E-commerce Back End

## Description
This application is the back end for an e-commerce site. It uses Express.js, Sequelize ORM, and PostgreSQL to provide a RESTful API for managing categories, products, tags, and product tags. This project is part of a challenge to build a comprehensive back end that supports CRUD operations for an e-commerce platform.

## Table of Contents
- [Description](#description)
- [Demo](#demo)
- [Instructions](#instructions)
- [Required Packages](#required-packages)
- [Installation](#installation)

## Demo
The following animation shows the application's GET routes to return all categories, all products, and all tags being tested in Insomnia:

![In Insomnia, the user tests “GET tags,” “GET Categories,” and “GET All Products.”.](./Assets/get-routes-13.mp4)

The following animation shows the application's GET routes to return a single category, a single product, and a single tag being tested in Insomnia:

![In Insomnia, the user tests “GET tag by id,” “GET Category by ID,” and “GET One Product.”](./Assets/get-findOne-13.mp4)

The following animation shows the application's POST, PUT, and DELETE routes for categories being tested in Insomnia:

![In Insomnia, the user tests “DELETE Category by ID,” “CREATE Category,” and “UPDATE Category.”](./Assets/post-put-delete-13.mp4)

## Instructions
1. Clone the repository.
2. Install the required packages.
3. Set up your PostgreSQL database.
4. Seed the database with test data.
5. Run the application.

## Required Packages
- `express`
- `sequelize`
- `pg`
- `dotenv`

## Installation
1. Clone the repository:
    ```sh
    git clone https://github.com/crob127/E-commerce-Back-End.git
    cd E-commerce-Back-End
    ```

2. Install the required packages:
    ```sh
    npm install
    ```

3. Create a `.env` file in the root directory and add your database credentials:
    ```
    DB_NAME='ecommerce_db'
    DB_USER='postgres'
    DB_PASSWORD=''
    ```

4. Create and seed the database:
    ```sh
    npx sequelize-cli db:create
    npx sequelize-cli db:migrate
    npx sequelize-cli db:seed:all
    ```

5. Start the application:
    ```sh
    npm start
    ```

For development, you can use `nodemon`:
    ```sh
    npm run dev
    ```

## Usage
Once the application is running, you can interact with the API using tools like Postman or Insomnia to perform CRUD operations on categories, products, tags, and product tags.

## Contributing
Feel free to submit issues and pull requests for improvements or bug fixes. Ensure your code adheres to the established style guidelines and is well-documented.

## License
This project is licensed under the MIT License.
