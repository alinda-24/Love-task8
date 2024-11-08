# 📚 **Creative Programming with Classes and File-Based Object Instantiation**

Welcome to your new programming task! In this series of exercises, you will delve into the world of Java programming with a focus on using file data to dynamically create objects, designing robust classes, and exercising your creative problem-solving skills in programming. The overarching theme we'll explore is the creation of a dynamic **Library Management System**.

## 🚀 **Learning Goals**

By the end of these exercises, you will:

1. **Using Data from Files to Instantiate Objects:**
   - Understand various file formats and parsing techniques.
   - Use Java file I/O classes to read data and convert it into object attributes.
   - Handle exceptions and ensure data integrity during object instantiation.

2. **Designing Classes:**
   - Identify class responsibilities and define clear interfaces.
   - Implement cohesive class structures with appropriate fields and methods.
   - Leverage design patterns to solve common problems and enhance class design.

3. **Programming Creatively:**
   - Explore different approaches to problem-solving and algorithm design.
   - Encourage experimentation and iteration to refine solutions.
   - Integrate user feedback and testing to improve program effectiveness and usability.

## 📝 **Exercises**

### 🧠 **Exercise 1: Understanding File Formats and Parsing** 

**Objective:**  
Explore theoretical aspects of file-based data extraction.

**Instructions:**  
- Describe the differences between CSV and JSON file formats. Why might one be preferred over the other in different scenarios?
- Discuss how data can be parsed from a text file in Java without using external libraries. Mention tools or classes you might employ.
  
_No code is required for this exercise._

---

### 🧩 **Exercise 2: Class Design Principles**

**Objective:**  
Solidify your understanding of effective class design.

**Instructions:**  
- Explain why it’s essential for a class to have well-defined responsibilities.
- Discuss how design patterns can help enhance class design, providing an example of one such pattern.
  
_No code is required for this exercise._

---

### 🔧 **Exercise 3: Basic File Parsing and Object Creation**

**Objective:**  
Implement basic file reading to instantiate objects in Java.

**Scenario:**  
You’re tasked with reading a list of books from a CSV file and creating a `Book` class for our library system.

**Instructions:**  
- Design the `Book` class with attributes such as `title`, `author`, `yearPublished`, and `ISBN`.
- Write a Java method `loadBooksFromFile(String filename)` that reads each line of a CSV file and creates a `Book` object for each entry, adding it to an ArrayList of Books.
  
_Sample CSV entry format:_  
`"The Great Gatsby, F. Scott Fitzgerald, 1925, 9780743273565"`

```java
public class Book {
    private String title;
    private String author;
    private int yearPublished;
    private String isbn;
    // Constructors, getters, and setters...
}

public ArrayList<Book> loadBooksFromFile(String filename) {
    // Implement file reading and parsing logic here
}
```

---

### 🔨 **Exercise 4: Designing the Library Class**

**Objective:**  
Integrate the `Book` class into a `Library` class and focus on class cohesion.

**Instructions:**  
- Design a `Library` class with methods to add books (`addBook`), list all books (`listBooks`), and search for a book by title (`findBookByTitle(String title)`).
- Consider using a `Map` to store books for faster search operations by title.

```java
public class Library {
    private Map<String, Book> books;
    // Implement addBook, listBooks, findBookByTitle, and other necessary methods.
}
```

---

### 💡 **Exercise 5: Dynamic Library with File-Driven Initialization**

**Objective:**  
Enhance the library system by dynamically reading and applying more complex data sets.

**Instructions:**  
- Extend your `loadBooksFromFile` method to handle possible parsing errors with graceful exception handling.
- Add a feature in `Library` class to update book details (like changing the year or correcting the title).

_Hint: Use a `try-catch` block to handle file I/O exceptions._

```java
// Enhance loadBooksFromFile with exception handling
```

---

### 🎨 **Exercise 6: Creative Enhancement**

**Objective:**  
Bring creativity into the design and implementation of your library system.

**Instructions:**  
- Add a feature to manage book loans and returns. Include a `User` class representing patrons of the library.
- Design a user interface (console-based) that allows interaction with the library system.
- Use user feedback to iterate and refine your system, ensuring it's user-friendly and robust.

```java
public class User {
    private String name;
    private List<Book> borrowedBooks;
    // Implement loanBook, returnBook, and other methods.
}
```

#### **Submission Requirements**

- Submit your Java source files and a README explaining how your library system works.
- Ensure your code is well-documented with Javadoc comments for all public classes and methods.
- Include sample input files used for testing.

Prepare to showcase your programming skills and creativity as you embark on designing and building a functional Library Management System! Happy coding! 🚀