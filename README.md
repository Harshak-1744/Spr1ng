# Spr1ng
## CRUD Operations in Spring Boot
CRUD operations using Spring Boot, a popular Java framework for building web applications. 
CRUD stands for Create, Read, Update, and Delete, which are the basic operations performed on data in most software applications.

## Database
* h2


# Issues 

## Issue Description

The project encountered an issue related to conflicting request mappings in the Spring MVC controller. The error message "This application has no explicit mapping for /error" was displayed when accessing a specific URL.

### Error Details

When attempting to fetch data by the "aname" value passed in the URL (e.g., http://localhost:8080/aliens/"harsha" ), the application showed an error message indicating "This application has no explicit mapping for /error, so you are seeing this as a fallback."

## Resolution

The issue was resolved by making the following changes in the controller code:

- The `@PathVariable` annotation for fetching aliens by name was modified to `@PathVariable("aname")`.

- The request mapping pattern for fetching aliens by name was changed to "/aliens/byName/{aname}" to ensure uniqueness and eliminate conflicts with other request mappings.

With these changes, the application successfully fetched data by the "aname" value passed in the URL.

## Documentation and Learning Resources

To understand the issue and its resolution, the following resources can be helpful:

- [Spring Framework Documentation](https://spring.io/): The official documentation for the Spring Framework provides comprehensive information about request mapping and handling in Spring MVC.

- [Spring Boot Documentation](https://spring.io/projects/spring-boot): If you are using Spring Boot for your application, the official Spring Boot documentation covers various aspects of developing web applications with Spring Boot, including request mapping.

- [Baeldung](https://www.baeldung.com/): Baeldung offers detailed tutorials and articles on Spring-related topics. to find specific guides on request mapping and conflict resolution on their website.

- [Spring Guides](https://spring.io/guides): Spring Guides provides practical, hands-on guides for working with Spring technologies. They cover various aspects of Spring development, including request mapping.

- [Stack Overflow](https://stackoverflow.com/): Stack Overflow is a popular question and answer platform where you can search for specific questions or issues related to Spring request mapping conflicts.


