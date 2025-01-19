# Product-Management-System

<h4>follwing steps for setup project </h4>

1) Create a Spring Boot Project.

    Use Spring Initializr to generate the project.
    Include dependencies: Spring Web, Spring Data JPA, MySQL Driver, and Spring Boot DevTools.
    Database Configuration
    
2) Configure the database in application.properties.
   # MySQL Configuration
        spring.datasource.url=jdbc:mysql://localhost:3306/databasename
        spring.datasource.username=yourusername
        spring.datasource.password=yourpassword
        spring.jpa.hibernate.ddl-auto=update
        spring.jpa.show-sql=true

  # Server Configuration
        server.port=8080

        
