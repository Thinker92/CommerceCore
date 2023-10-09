# E-commerce Back End

## Table of Contents

- [Description](#description)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Walkthrough Video](#walkthrough-video)

## Description

This project provides the back end for an e-commerce website. It uses Express.js API and Sequelize to interact with a MySQL database.

## Installation

1. Clone the repository to your local machine.
2. Navigate to the project directory.
3. Run `npm install` to install all dependencies.
4. Create a `.env` file for environment variables with your MySQL user, password, and database name.
5. Run `npm run seed` to populate the database.
6. Run `node server.js` to start the application.

## Usage

This application exposes API endpoints for managing categories, products, and tags of an e-commerce website. You can test the API routes using Postman or Insomnia.

### Categories

- **GET all categories**: `http://localhost:3001/api/categories`
- **GET a single category by ID**: `http://localhost:3001/api/categories/:id`
- **POST a new category**: `http://localhost:3001/api/categories`
  - Body: `{"category_name": "Electronics"}`
- **PUT update a category by ID**: `http://localhost:3001/api/categories/:id`
  - Body: `{"category_name": "Electronics and Gadgets"}`
- **DELETE a category by ID**: `http://localhost:3001/api/categories/:id`

### Products

- **GET all products**: `http://localhost:3001/api/products`
- **GET a single product by ID**: `http://localhost:3001/api/products/:id`
- **POST a new product**: `http://localhost:3001/api/products`
  - Body: `{"product_name": "Laptop", "price": 1000.00, "stock": 5, "tagIds": [1, 2]}`
- **PUT update a product by ID**: `http://localhost:3001/api/products/:id`
  - Body: `{"product_name": "High-end Laptop", "price": 2000.00}`
- **DELETE a product by ID**: `http://localhost:3001/api/products/:id`

### Tags

- **GET all tags**: `http://localhost:3001/api/tags`
- **GET a single tag by ID**: `http://localhost:3001/api/tags/:id`
- **POST a new tag**: `http://localhost:3001/api/tags`
  - Body: `{"tag_name": "Seasonal"}`
- **PUT update a tag by ID**: `http://localhost:3001/api/tags/:id`
  - Body: `{"tag_name": "Holiday Seasonal"}`
- **DELETE a tag by ID**: `http://localhost:3001/api/tags/:id`

## Contributing

1. Fork the project.
2. Create a new branch (`git checkout -b feature/fooBar`).
3. Commit your changes (`git commit -am 'Add some fooBar'`).
4. Push to the branch (`git push origin feature/fooBar`).
5. Create a new Pull Request.

## License

This project is licensed under the terms of the MIT License. 

## Walkthrough Video

For a complete walkthrough of the application, please refer to the following video:

[CommerceCore Walkthrough Video](./CommerceCore-walkthrough.webm)

