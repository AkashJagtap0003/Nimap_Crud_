Sure, here's the complete content for a single `README.md` file:

```markdown
# Nimap Infotech CRUD Example

This is a Spring Boot application that demonstrates CRUD operations for managing categories and products. The project also showcases the use of JPA & Hibernate, server-side pagination, and the establishment of a one-to-many relationship between Category and Products.

## Features

- Category CRUD operations
- Product CRUD operations
- One-to-many relationship between Category and Products
- Server-side pagination
- Fetching single product details along with respective category details

## Technologies Used

- Spring Boot
- Spring Data JPA
- Hibernate
- MySQL
- Lombok
- Maven
- RESTful APIs

## Getting Started

### Prerequisites

- JDK 11 or higher
- Maven
- MySQL database

### Installation

1. Clone the repository
   ```sh
   git clone https://github.com/AkashJagtap0003/Nimap_Crud_.git
   ```

2. Navigate to the project directory
   ```sh
   cd Nimap_Crud_
   ```

3. Update MySQL database configuration in `src/main/resources/application.properties`
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/your_database_name
   spring.datasource.username=your_username
   spring.datasource.password=your_password
   spring.jpa.hibernate.ddl-auto=update
   ```

4. Build the project using Maven
   ```sh
   mvn clean install
   ```

5. Run the application
   ```sh
   mvn spring-boot:run
   ```

## API Endpoints

### Category CRUD Operations

1. **Get all categories**
   ```http
   GET /api/categories?page=0
   ```

2. **Create a new category**
   ```http
   POST /api/categories
   Content-Type: application/json

   {
     "name": "Electronics"
   }
   ```

3. **Get category by ID**
   ```http
   GET /api/categories/{id}
   ```

4. **Update category by ID**
   ```http
   PUT /api/categories/{id}
   Content-Type: application/json

   {
     "name": "Updated Category"
   }
   ```

5. **Delete category by ID**
   ```http
   DELETE /api/categories/{id}
   ```

### Product CRUD Operations

1. **Get all products**
   ```http
   GET /api/products?page=0
   ```

2. **Create a new product**
   ```http
   POST /api/products
   Content-Type: application/json

   {
     "name": "iPhone",
     "price": 999.99,
     "category": {
       "id": 1
     }
   }
   ```

3. **Get product by ID**
   ```http
   GET /api/products/{id}
   ```

4. **Update product by ID**
   ```http
   PUT /api/products/{id}
   Content-Type: application/json

   {
     "name": "Updated Product",
     "price": 1099.99,
     "category": {
       "id": 1
     }
   }
   ```

5. **Delete product by ID**
   ```http
   DELETE /api/products/{id}
   ```

## Usage

### Pagination

To fetch paginated results, include the `page` parameter in your GET requests. The default page size is set to 10.

### Example Requests

1. **Get the first page of categories**
   ```http
   GET /api/categories?page=0
   ```

2. **Get the second page of products**
   ```http
   GET /api/products?page=1
   ```

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

Akash Jagtap - jagtapakash8419@gmail.com

Project Link: [https://github.com/AkashJagtap0003/Nimap_Crud_](https://github.com/AkashJagtap0003/Nimap_Crud_)
```

Feel free to replace placeholders like `your_database_name`, `your_username`, `your_password`, and `akash.jagtap@example.com` with your actual details. This `README.md` file contains all the information in one place.
