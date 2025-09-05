# 🧑‍💻 Employee Maintenance System

This is a **full-stack employee management system** built using **Java, Spring Boot, MySQL, HTML, CSS, and JavaScript**.  
It allows users to **add, view, update, and delete employees** with a clean separation of **back-end (APIs)** and **front-end (UI)**.

---

## ✨ Features
- **Create** → Add new employees  
- **Read** → View employee list  
- **Update** → Modify employee details  
- **Delete** → Remove employees  
- **RESTful APIs** → Back-end APIs exposed via Spring Boot  
- **AJAX-based Front-End** → UI connects to back-end using APIs  

---

## 🛠️ Tech Stack
- **Back-End**: Java, Spring Boot, Spring Data JPA  
- **Database**: MySQL (via XAMPP)  
- **Front-End**: HTML, CSS, JavaScript, Bootstrap 5, jQuery, SweetAlert2  
- **Server**: Apache (XAMPP)  
- **IDE**: Eclipse  
- **Build Tool**: Maven  

---

## 📁 Project Structure

The project is divided into two main parts: **Back-End (Spring Boot)** and **Front-End (Apache in XAMPP)**.

### 🔹 Back-End: `employeecrud/`
This is the **Spring Boot project** responsible for handling business logic and exposing REST APIs.

  - `src/main/java/com/employee/crud/` → Contains the Java source code  
  - `CrudApplication.java` → Entry point of the Spring Boot application  
  - `controller/EmployeeController.java` → Handles REST API requests (CRUD operations)  
  - `entity/Employee.java` → Entity class mapped to the database table  
  - `src/main/resources/` → Contains configuration files  
  - `application.properties` → Database connection details, server port, Hibernate settings  
  - `pom.xml` → Maven build file, used to manage dependencies and plugins  

---

### 🔹 Front-End: `EmployeeUI/`
This is the **UI part** of the project, served via **Apache (XAMPP)**. It communicates with the back-end through AJAX calls.

- **`index.html`** → Main user interface page (employee management dashboard)  
- **`css/`** → Stylesheets for UI design and layout  
- **`js/`** → JavaScript + AJAX logic to fetch/update data from APIs  
- **`image/`** → Image assets like logos and icons  

---

## 🚀 How to Run the Application

### Step 1: Start XAMPP
- Open **XAMPP Control Panel**  
- Start **MySQL** and **Apache**  
- Wait until both turn **green**  

### Step 2: Run Back-End (Spring Boot)
- Open the project in **Eclipse**  
- In Project Explorer, right-click `CrudApplication.java` → **Run As > Spring Boot App**  
- Confirm that the back-end is working by opening:  
  👉 [http://localhost:8086/api/employee](http://localhost:8086/api/employee)  

### Step 3: Set Up Front-End (EmployeeUI)
- Copy the **EmployeeUI** folder into your **XAMPP htdocs** directory  
  (usually `C:\xampp\htdocs\`)  

### Step 4: Run Front-End
- Open your browser and go to:  
  👉 [http://localhost:8080/EmployeeUI/](http://localhost:8080/EmployeeUI/)  
- The UI will fetch data from the back-end running at  
  👉 [http://localhost:8086/api/employee](http://localhost:8086/api/employee)  

✅ Now you can **Add, Edit, Delete, and View employees** 🎉  

---

## 📌 Notes
- Always start **XAMPP (MySQL + Apache)** before running the app  
- Run the **back-end first**, then the **front-end**  
- If Apache runs on another port, update AJAX URLs in `index.html`  

---

## 📜 License
This project is open-source and available under the **MIT License**  
