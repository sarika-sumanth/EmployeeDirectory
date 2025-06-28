# EmployeeDirectory

A simple **Spring Boot** application that provides basic **CRUD operations** for managing employees.

## 🚀 Features

- View all employees
- Add a new employee
- Update existing employee details
- Delete an employee
- REST API with JSON support
- Pagination and sorting support (optional)

## 🛠️ Technologies Used

- Java 17+ (or compatible)
- Spring Boot
- Spring Data JPA
- Hibernate
- RESTful APIs
- H2 / MySQL (based on config)
- Maven


## 📁 Project Structure

EmployeeDirectory/
├── .gitattributes
├── .gitignore
├── HELP.md
├── mvnw / mvnw.cmd # Maven wrapper scripts
├── pom.xml # Maven configuration
├── README.md

├── .idea/ # IntelliJ IDEA config files
│ └── ... # .xml settings files
│
├── .mvn/
│ └── wrapper/
│ └── maven-wrapper.properties

├── src/
│ ├── main/
│ │ ├── java/
│ │ │ └── com/example/demo/
│ │ │ ├── DemoApplication.java # Main Spring Boot app
│ │ │
│ │ │ ├── dao/
│ │ │ │ ├── EmployeeDAO.java # DAO interface
│ │ │ │ └── EmployeeDAOImp.java # DAO implementation
│ │ │
│ │ │ ├── entity/
│ │ │ │ └── Employee.java # JPA entity
│ │ │
│ │ │ ├── rest/
│ │ │ │ └── EmployeeRestController.java # REST controller
│ │ │
│ │ │ └── service/
│ │ │ ├── EmployeeService.java # Service interface
│ │ │ └── EmployeeServiceImpl.java # Service implementation
│ │
│ │ └── resources/
│ │ ├── application.properties # Spring config
│ │ ├── static/ # (Empty - for web assets)
│ │ └── templates/ # (Empty - for Thymeleaf if needed)
│
│
│ └── test/
│ └── java/com/example/demo/
│ └── DemoApplicationTests.java # Basic test class
│
├── target/ # Build output (ignored in Git)
└── ...



## Run the built JAR

java -jar target/employee-directory-0.0.1-SNAPSHOT.jar


## API Endpoints

| Method | Endpoint         | Description           |
| ------ | ---------------- | --------------------- |
| GET    | `/employee`      | Get all employees     |
| GET    | `/employee/{id}` | Get employee by ID    |
| POST   | `/employee`      | Add a new employee    |
| PUT    | `/employee`      | Update an employee    |
| DELETE | `/employee/{id}` | Delete employee by ID |



## Example JSON

{
  "firstName": "John",
  "lastName": "Doe",
  "email": "john.doe@example.com"
}





## 📄 License
This project is open-source under the MIT License.

