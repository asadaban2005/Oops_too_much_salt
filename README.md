📄 Review-2 Compliance Summary

✔ Core features implemented
✔ Full OOP usage
✔ Robust error handling
✔ Clean modular structure
✔ GUI event handling
✔ Data validation
✔ Well-documented README
✔ GitHub ready for submission


🍲 Oops Too Much Salt

Oops Too Much Salt is a Java Swing–based recipe management application built using core Object-Oriented Programming (OOP) principles.
The project demonstrates clean architecture, modular design, GUI interaction, data validation, exception handling, and database integration.

📌 Project Objective

To design and implement a robust Java GUI application that allows users to manage recipes efficiently while showcasing:

Strong OOP concepts

Clean code practices

Modular architecture

Error handling & validation

GUI event handling

🧱 Project Folder Structure
oopstoomuchsalt/
│
├── README.md
│
└── src/
    ├── db/
    │   ├── DatabaseConnection.java
    │   └── DBBase.java
    │
    ├── models/
    │   ├── Recipe.java
    │   ├── VegRecipe.java
    │   ├── NonVegRecipe.java
    │   └── User.java
    │
    ├── services/
    │   ├── IRecipeService.java
    │   ├── RecipeService.java
    │   └── UserService.java
    │
    ├── exceptions/
    │   ├── RecipeException.java
    │   └── RecipeRuntimeException.java
    │
    └── gui/
        ├── MainWindow.java
        └── RecipeForm.java

🧠 OOP Concepts Implemented
Concept	Usage
Encapsulation	Private fields with getters/setters in models
Inheritance	VegRecipe & NonVegRecipe extend Recipe
Abstraction	IRecipeService interface
Polymorphism	Service methods operate on Recipe objects
Exception Handling	Custom checked & unchecked exceptions
Separation of Concerns	GUI, Service, Model, DB layers
⚙️ Core Features

📋 View all recipes

➕ Add new recipes

✏️ Edit existing recipes

🗑 Delete recipes

🔍 Search & filter recipes

🪟 Java Swing GUI

🧩 Modular service-based architecture

🛡 Error Handling & Robustness

Graceful handling of:

Empty input fields

Database connection failures

Invalid user actions

Custom exceptions:

RecipeException

RecipeRuntimeException

Application does not crash on runtime errors

✅ Data Validation

Client-side validation using Swing:

Empty fields blocked

Invalid inputs prevented

Server-side validation:

Database query safety using PreparedStatement

🔗 Integration of Components

GUI interacts only with Service layer

Services interact with DB layer

Models remain independent and reusable

Clean separation ensures easy testing & maintenance

🧪 Event Handling & Processing

Optimized Swing event listeners

Proper delegation of GUI actions

Responsive UI behavior

🛠 Technologies Used

Java (JDK 17+)

Java Swing

JDBC

MySQL

IntelliJ IDEA / VS Code

🗄 Database Setup (Required for Full Functionality)
1️⃣ Install MySQL

Make sure MySQL Server is installed and running.

2️⃣ Create Database & Table
CREATE DATABASE oopstoomuchsalt;
USE oopstoomuchsalt;

CREATE TABLE recipes (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255),
    ingredients TEXT,
    instructions TEXT
);

3️⃣ Update DB Credentials

Edit:

db/DatabaseConnection.java

private static final String USER = "root";
private static final String PASSWORD = "your_password";


⚠️ If MySQL is not running, the application handles the error gracefully.

▶️ How to Run

Open project in IDE

Add MySQL Connector JAR to classpath

Run:

gui.MainWindow


👤 Author

Asad Aban Arif & Tanmay shrivastava
B.Tech CSE (AI & ML)
Galgotias University

If you want, I can now:

✔️ Verify this against your rubric

✔️ Help you write Review-2 explanation lines

✔️ Do a final submission checklist

Just say the word.
