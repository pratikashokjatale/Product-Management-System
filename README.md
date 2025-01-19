# Product-Management-System follwing steps for setup project 



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


3) Add dependencies
   #dependencies Configuration
   
       <dependencies>
        		<dependency>
        			<groupId>org.springframework.boot</groupId>
        			<artifactId>spring-boot-starter-data-jpa</artifactId>
        		</dependency>
        		<dependency>
        			<groupId>org.springframework.boot</groupId>
        			<artifactId>spring-boot-starter-web</artifactId>
        		</dependency>
        
        		<dependency>
        			<groupId>org.springframework.boot</groupId>
        			<artifactId>spring-boot-devtools</artifactId>
        			<scope>runtime</scope>
        			<optional>true</optional>
        		</dependency>
        		<dependency>
        			<groupId>com.mysql</groupId>
        			<artifactId>mysql-connector-j</artifactId>
        			<scope>runtime</scope>
        		</dependency>
        		<dependency>
        			<groupId>org.springframework.boot</groupId>
        			<artifactId>spring-boot-starter-tomcat</artifactId>
        			<scope>provided</scope>
        		</dependency>
        		<dependency>
        			<groupId>org.springframework.boot</groupId>
        			<artifactId>spring-boot-starter-test</artifactId>
        			<scope>test</scope>
        		</dependency>
	    </dependencies>    

<h1>Testing Category Api in Postman</h1>

GET all the categories
     			   
	     http://localhost:8080/api/categories?page=3

POST - create a new category

		   	
	http://localhost:8080/api/categories


 GET category by Id

   	
	http://localhost:8080/api/categories/{di}

 PUT - update category by id

 	
	http://localhost:8080/api/categories/{di}

 DELETE - Delete category by id

 	http://localhost:8080/api/categories/{di}

 <h1>Testing Products Api in Postman</h1>

 GET all the products
 			
    http://localhost:8080/api/products?page=2

POST - create a new product


	 http://localhost:8080/api/products

  GET product by Id


 	 http://localhost:8080/api/products/{di}

   PUT - update product by id


 	  http://localhost:8080/api/products/{di}

 DELETE - Delete product by id
 		

	http://localhost:8080/api/products/{di}
         
