# **Application.properties**

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/"DataBase_name"
spring.datasource.username="username"
spring.datasource.password="password"
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.jpa.show-sql=true
spring.jpa.hibernate.ddl-auto=update
```

# MySQL Database Configuration

This repository contains the configuration properties for connecting to a MySQL database in a Spring Boot application. These properties are defined in the `application.properties` file.

## Configuration Steps

1. Open the `application.properties` file located in the project's resources folder.

2. Update the following configuration properties according to your MySQL database setup:

   - `spring.datasource.url`: Specifies the URL for the MySQL database connection. Make sure to replace `localhost:3306/DataBase_name` with your MySQL server information and database name.
   
   - `spring.datasource.username`: Specifies the username for connecting to the MySQL database. Replace `username` with your actual username.
   
   - `spring.datasource.password`: Specifies the password for connecting to the MySQL database. Replace `password` with your actual password.
   
   - `spring.datasource.driver-class-name`: Specifies the JDBC driver class for the MySQL database. No changes are required for the provided value.
   
   - `spring.jpa.show-sql`: Enables the printing of SQL statements in the console. This can be useful for debugging. No changes are required for the provided value.
   
   - `spring.jpa.hibernate.ddl-auto`: Specifies the behavior of Hibernate for database schema generation. The provided value `update` automatically creates or updates the schema based on the entity classes. Use with caution in production.
   
3. Save the `application.properties` file with the updated configuration.

4. Start the Spring Boot application. It will now connect to the MySQL database using the specified configuration.

## Additional Information

- The `spring.jpa.show-sql=true` property enables the printing of SQL statements in the console. This can be useful for debugging and understanding the executed SQL queries.

- The `spring.jpa.hibernate.ddl-auto=update` property controls the database schema generation by Hibernate. It automatically creates or updates the schema based on the entity classes. Be cautious when using `update` in production.




