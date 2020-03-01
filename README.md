# Spring Boot Shopping Cart Web App

## About
The idea was to build some basic shopping cart web app for Ethoca.

It was made using **Spring Boot**, **Spring Data JPA**, **Spring Data REST**. 
Database is in memory **H2**.

Users can shop for products. Each user has his own shopping cart.
Checkout is transactional.

## Configuration

### Configuration Files

Folder **src/resources/** contains config files for **shopping-cart** Spring Boot application.

* **src/resources/application.properties** - main configuration file.

## How to run

Once the app starts, go to the web browser and visit `http://localhost:8070/products`

## Tests

Tests can be run by executing following command from the root of the project:

```bash
$ mvn test
```

## Helper Tools

### HAL REST Browser

Go to the web browser and visit `http://localhost:8070/`

### H2 Database web interface

Go to the web browser and visit `http://localhost:8070/h2-console`

In field **JDBC URL** put 
```
jdbc:h2:mem:shopping_cart_db
```

In `/src/main/resources/application.properties` file it is possible to change both
web interface url path, as well as the datasource url.
