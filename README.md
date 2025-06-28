Sure! Here's the **complete and clean `README.md`** file for your **EmployeeDirectory Spring Boot CRUD project**, with proper formatting that works perfectly on GitHub (including fixed project structure and code blocks).

---

```markdown
# EmployeeDirectory

A simple **Spring Boot** application that provides basic **CRUD operations** for managing employees.

---

## 🚀 Features

- View all employees
- Add a new employee
- Update existing employee details
- Delete an employee
- REST API with JSON support
- Pagination and sorting support (optional)

---

## 🛠️ Technologies Used

- Java 17+ (or compatible)
- Spring Boot
- Spring Data JPA
- Hibernate
- RESTful APIs
- H2 / MySQL (based on config)
- Maven

---

## 📁 Project Structure

```

EmployeeDirectory/
├── .gitattributes
├── .gitignore
├── HELP.md
├── mvnw
├── mvnw\.cmd                       # Maven wrapper scripts
├── pom.xml                        # Maven configuration
├── README.md

├── .idea/                         # IntelliJ IDEA config files
│   └── ...                        # .xml project settings

├── .mvn/
│   └── wrapper/
│       └── maven-wrapper.properties

├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/example/demo/
│   │   │       ├── DemoApplication.java              # Main Spring Boot app
│   │   │       ├── dao/
│   │   │       │   ├── EmployeeDAO.java              # DAO interface
│   │   │       │   └── EmployeeDAOImp.java           # DAO implementation
│   │   │       ├── entity/
│   │   │       │   └── Employee.java                 # JPA entity
│   │   │       ├── rest/
│   │   │       │   └── EmployeeRestController.java   # REST controller
│   │   │       └── service/
│   │   │           ├── EmployeeService.java          # Service interface
│   │   │           └── EmployeeServiceImpl.java      # Service implementation
│   │   └── resources/
│   │       ├── application.properties                # Spring configuration
│   │       ├── static/                               # (Optional) Web assets
│   │       └── templates/                            # (Optional) Thymeleaf templates
│   └── test/
│       └── java/com/example/demo/
│           └── DemoApplicationTests.java             # Unit test

├── target/                                            # Build output (Git ignored)
└── ...

````

---

## ▶️ How to Run the App

### 🧪 Using Maven

```bash
mvn clean install
mvn spring-boot:run
````

### 🚀 Run the built JAR

```bash
java -jar target/employee-directory-0.0.1-SNAPSHOT.jar
```

---

## 🔗 API Endpoints

| Method | Endpoint         | Description           |
| ------ | ---------------- | --------------------- |
| GET    | `/employee`      | Get all employees     |
| GET    | `/employee/{id}` | Get employee by ID    |
| POST   | `/employee`      | Add a new employee    |
| PUT    | `/employee`      | Update an employee    |
| DELETE | `/employee/{id}` | Delete employee by ID |

---

## 📦 Example JSON

```json
{
  "firstName": "John",
  "lastName": "Doe",
  "email": "john.doe@example.com"
}
```

---

## ⚙️ Configuration

Default H2 setup in `application.properties`:

```properties
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.driver-class-name=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.h2.console.enabled=true
```

You can switch to MySQL by updating:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/employeedb
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
```

---

## 🧪 Testing

You can test the API endpoints using tools like:

* **Postman**
* **cURL**
* Swagger (if configured)

---

## 📄 License

This project is open-source under the **MIT License**.

---

## 🙋‍♂️ Author

**Sumanth Sarika**
[GitHub: sarika-sumanth](https://github.com/sarika-sumanth)

---

````

---
