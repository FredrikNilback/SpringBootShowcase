Keep in mind if you want to use this showcase to test you will need to start up a database, and run the following MySQL script: 
CREATE DATABASE my_database;
USE my_database;

You will also need to provide the application.properties, typically under src/main/java/dev/your_name/application_name/resources/application.properties.
spring.application.name=application_name
spring.datasource.url=jdbc:mysql://localhost:3306/my_database?useSSL=false&serverTimezone=UTC  adjust for your database port. 
spring.datasource.username=your_database_username
spring.datasource.password=your_database_password
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=false
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect
