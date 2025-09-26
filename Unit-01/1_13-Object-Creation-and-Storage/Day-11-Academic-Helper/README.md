# 📝 Programming Exercise: The **`AcademicHelper`** Utility Class

## **Goal**

You will create a utility class named `AcademicHelper` with only **static methods** and proper documentation. You will also create a `Runner` class that uses the `AcademicHelper` methods as well as create a `Student` object using a provided class. This exercise reinforces concepts from Unit 1, including:

* Primitive Data Types (`int`, `double`) and Casting (1.2, 1.4, 1.6)
* The `String` class (1.7)
* Documentation with comments (1.8)
* **Static Methods** (1.12)
* The **`Math` Class** methods (1.11)
* Object Creation and Storage (1.13)

## **Scenario**

You are creating a helpful, universal utility class that any part of a larger school application can use *without* needing to create an object. This is a common design pattern for utility functions, and it requires all methods to be declared as `static`. You will also create a `Student` class to represent a student and a `Runner` class to tie everything together by taking user input.

## **Requirements**

You must implement the following **four static methods** inside the `AcademicHelper` class and write proper documentation, and in the `Runner` file you will collect user input to use the methods you've created. Finally, you will create a `Student` object to put it all together.

### `calculateAverage`
* **Parameters:** `int score1`, `int score2`, `int score3`
* **Return Type:** `double`
* **Description:** Calculates the average of the three integer scores (each out of 100). **Must use casting** to ensure the division results in a `double` value (e.g., $85/3$ should be $28.333...$, not $28$).
* **Example:** `calculateAverage(80, 88, 91)` returns `86.33333...`
* **Concepts:** `int`, `double`, Casting, Arithmetic

### `getHigherScore`
* **Parameters:** `int a`, `int b`
* **Return Type:** `int`
* **Description:** Returns the larger of the two given scores. **Must use a static method from the `Math` class.**
* **Example:** `getHigherScore(91, 78)` returns `91`
* **Concepts:** `Math.max`, `int`, Static Methods

### `roundToNearestWhole`
* **Parameters:** `double percentage`
* **Return Type:** `int`
* **Description:** Converts a decimal percentage (e.g., $87.5$) into a rounded whole number grade (e.g., $88$). **Must use the add 0.5 method** and casting to return an `int`.
* **Example:** `roundToNearestWhole(86.33333)` returns `86`
* **Concepts:** `double`, `int`, Casting

### `createGradeReport`
* **Parameters:** `String studentName`, `double finalScore`
* **Return Type:** `String`
* **Description:** Returns a single String containing a simple, personalized report.
* **Example:** `createGradeReport("Mr. Fritz", 86.3333333)` returns `"Report for Mr. Fritz: Final Score is 86"`
* **Concepts:** `String` concatenation, `double`

---

## **Starter Code**

The files needed are all provided for you. Only the `Student` class is complete and does not need to be modified.

## Javadocs Example
This is an example of a proper Javadoc comment that you can include in your code. It explains the purpose of the method, its parameters, and what it returns.

```java
  /**
   * Calculates the square of a given number.
   * @param number The number to be squared.
   * @return The square of the number.
   */
  public static int getSquare(int number) {
      return number * number;
  }
```

## Runner File

Your `Runner` file should accomplish the following:

1. Collect the following user input:
    - name
    - three separate grades
2. Calculate the average grade using the appropriate `AcademicHelper` method
3. Print the average grade.
4. Pass the name and average grade to the `createGradeReport` method and print the returned `String`
5. Use the `roundToNearestWhole` method to store the rounded percentage
6. Create a `Student` object using the name and rounded final grade
7. Print confirmation of creating the object

## Example

An example of this program running can be found [here](https://codehs.com/sandbox/stefanfritz/academic-helper-key/run)
