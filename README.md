# Workshop JavaFX JDBC

[![NPM](https://img.shields.io/npm/l/react)](https://github.com/IannNS/workshop-javafx-jdbc/blob/main/LICENSE) 

## About the project

This project is a desktop application developed during a Java training workshop. The application consists of a system for managing sellers and departments (CRUD), built with **JavaFX** and **JDBC**.

The project implements the MVC (Model-View-Controller) pattern and demonstrates manual dependency injection and database handling without frameworks like Hibernate, focusing on the core understanding of JDBC and JavaFX.

## Conceptual Model
![Conceptual Model](https://github.com/acenelio/workshop-javafx-jdbc/raw/master/db.png)

## Technologies used

- Java 11+
- JavaFX
- JDBC
- MySQL
- Scene Builder

## How to run the project

### Prerequisites
- Java JDK 11 or higher
- MySQL Server
- **JavaFX SDK** (See below)

### Database Setup
1. Make sure your MySQL service is running.
2. Run the SQL script located in the project folder (if available) or create a database named `coursejdbc`.
3. Configure your connection in the `db.properties` file located in the source root.

### JavaFX SDK Configuration
**Important:** To run this application, you must download the **JavaFX SDK** compatible with your operating system.

1. Download the SDK from [Gluon](https://gluonhq.com/products/javafx/).
2. Extract the SDK to a folder on your computer (e.g., `C:\java-libs\javafx-sdk`).
3. When running the application (or the test class), you must add the following **VM Arguments** to your Run Configuration:

```bash
--module-path "\path\to\javafx-sdk\lib" --add-modules javafx.controls,javafx.fxml
