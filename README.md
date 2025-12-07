# Oops Too Much Salt

## Project Overview

“Oops Too Much Salt” is a mini recipe-sharing platform built in Java. Users can **add, edit, delete, and search recipes** with ingredients and instructions using a modern graphical user interface (GUI) built with Swing. Recipes are stored in a **MySQL database** using JDBC for demonstration purposes.

---

## Project Features

* Add new recipes with name, ingredients, and instructions
* Edit existing recipes
* Delete recipes
* Search recipes by name or ingredients
* Styled, professional GUI for better user experience
* OOP-based layered architecture
* JDBC integration with MySQL for persistent storage

---

## Project Structure

```
OopstoomuchSalt
 ┣ README.md
 ┗ src
   ┣ db
   │ ┣ DatabaseConnection.java
   │ ┗ DBBase.java
   ┣ models
   │ ┣ Recipe.java
   │ ┣ VegRecipe.java
   │ ┣ NonVegRecipe.java
   │ ┗ User.java
   ┣ services
   │ ┣ IRecipeService.java
   │ ┣ RecipeService.java
   │ ┗ UserService.java
   ┣ exceptions
   │ ┣ RecipeException.java
   │ ┗ RecipeRuntimeException.java
   ┗ gui
     ┣ MainWindow.java
     ┗ RecipeForm.java

```
🧠 OOP Concepts Used
Concept	Where Used
Encapsulation	models class fields
Inheritance	VegRecipe, NonVegRecipe extend Recipe
Polymorphism	overridden methods
Abstraction	IRecipeService interface
Exceptions	custom exceptions package
MVC Layer	gui / services / models / db

---

## Requirements

* Java JDK 17+
* MySQL Server
* IDE or editor (VS Code, IntelliJ, Eclipse) or terminal for compiling and running
* No external libraries are required

---

## Setup Instructions

1. **Clone or download the repository** into your local machine.
2. **Set up MySQL Database**:

   * Create a database named `oopstoomuchsalt`
   * Update `DatabaseConnection.java` if your DB username/password are different
3. **Navigate to the `src` folder** in your terminal or IDE.
4. **Compile the project**:

```bash
javac db/*.java models/*.java services/*.java gui/*.java
```

5. **Run the application**:

```bash
java gui.MainWindow
```

> The GUI window will open, allowing users to add, edit, delete, and search recipes.

---

## Project Review

Students implemented **core Java and OOP principles**, defined a **clear project structure**, designed the **database schema**, established **JDBC connectivity**, and developed **classes for database operations**. This allows the project to evolve into a **fully database-backed, professional Java application**.

---

## Future Improvements

* Multi-user login/signup system
