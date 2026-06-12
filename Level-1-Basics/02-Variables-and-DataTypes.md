# 02 - Variables and Data Types

In this lesson, you'll learn how to **store and manage data** in Java using variables and data types.

## 🎯 Learning Objectives

By the end of this lesson, you will:
- ✅ Understand what variables are
- ✅ Know how to declare variables
- ✅ Understand primitive data types
- ✅ Use variables in your programs
- ✅ Know the differences between data types

---

## 🧠 What is a Variable?

A **variable** is a named container that stores a value. Think of it like a labeled box:

```
Box Label: age
Box Contents: 25
```

In code:
```java
int age = 25;
```

**Why use variables?**
- Store information for later use
- Make code readable and maintainable
- Manipulate data during program execution

---

## 📝 Declaring Variables

### Syntax:
```java
dataType variableName = value;
```

### Examples:
```java
int age = 25;              // Whole number
double height = 5.9;       // Decimal number
String name = "Ahad";      // Text
boolean isStudent = true;  // True or False
```

**Breaking it down:**
- `int` - The data type (integer/whole number)
- `age` - The variable name
- `=` - Assignment operator
- `25` - The value being stored

---

## 🏷️ Primitive Data Types

Java has **8 primitive data types**. Here are the most important:

### 1. **Integer Types** (Whole Numbers)

| Type | Size | Range | Example |
|------|------|-------|---------|
| `byte` | 1 byte | -128 to 127 | `byte b = 100;` |
| `short` | 2 bytes | -32,768 to 32,767 | `short s = 5000;` |
| `int` | 4 bytes | -2.1B to 2.1B | `int age = 25;` |
| `long` | 8 bytes | Very large numbers | `long bigNum = 1234567890L;` |

**Use `int` most of the time. Use `long` for very big numbers.**

### 2. **Decimal Types** (Floating Point Numbers)

| Type | Size | Precision | Example |
|------|------|-----------|---------|
| `float` | 4 bytes | 6-7 digits | `float price = 19.99f;` |
| `double` | 8 bytes | 15-16 digits | `double height = 5.9;` |

**Use `double` most of the time. It's more accurate.**

### 3. **Character Type**

| Type | Size | Example |
|------|------|---------|
| `char` | 2 bytes | `char grade = 'A';` |

**Important:** Use single quotes `'A'`, not double quotes.

### 4. **Boolean Type** (True/False)

| Type | Size | Example |
|------|------|---------|
| `boolean` | 1 bit | `boolean isActive = true;` |

---

## 🔤 String Data Type (Non-Primitive)

`String` is a special type that stores text. Unlike primitive types, it's an object:

```java
String name = "Ahad Rahman";
String city = "Dhaka";
String message = "Hello, Java!";
```

**Important:** Use double quotes `"text"` for Strings, not single quotes.

---

## 💻 Complete Example Program

Here's a program using different variables:

```java
public class VariablesDemo {
    public static void main(String[] args) {
        
        // Integer variables
        int age = 25;
        int yearOfBirth = 2000;
        
        // Decimal variables
        double height = 5.9;
        double gpa = 3.75;
        
        // String variables
        String name = "Ahad Rahman";
        String city = "Dhaka";
        
        // Boolean variable
        boolean isStudent = true;
        
        // Character variable
        char grade = 'A';
        
        // Print all variables
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
        System.out.println("Height: " + height + " feet");
        System.out.println("City: " + city);
        System.out.println("GPA: " + gpa);
        System.out.println("Is Student: " + isStudent);
        System.out.println("Grade: " + grade);
    }
}
```

**Output:**
```
Name: Ahad Rahman
Age: 25
Height: 5.9 feet
City: Dhaka
GPA: 3.75
Is Student: true
Grade: A
```

---

## 📋 Variable Naming Rules

Java has specific rules for naming variables:

### ✅ Valid Names:
- `age`
- `myAge`
- `_privateVar`
- `var1`
- `userName`

### ❌ Invalid Names:
- `123age` - Can't start with a number
- `my-age` - Can't use hyphens
- `my age` - Can't have spaces
- `class` - Can't use reserved words
- `int` - Already a data type

### Best Practices:
- Use **camelCase**: `myVariableName` (not snake_case or SCREAMING_CASE)
- Use **descriptive names**: `studentAge` not `x`
- Use **meaningful names**: `numberOfStudents` not `n`

---

## 🔄 Variable Assignment

Once a variable is declared, you can change its value:

```java
int age = 25;           // Declare and assign
System.out.println(age); // Output: 25

age = 26;               // Change the value
System.out.println(age); // Output: 26

age = age + 1;          // Use old value to compute new value
System.out.println(age); // Output: 27
```

---

## 🔒 Constants

Use `final` keyword to create variables that **cannot be changed**:

```java
final int MAX_STUDENTS = 30;
final double PI = 3.14159;

MAX_STUDENTS = 40;  // ❌ ERROR - Cannot change a final variable
```

**Use constants for values that never change in your program.**

---

## 📊 Data Type Comparison Table

| Type | Use For | Size | Range/Example |
|------|---------|------|----------------|
| `int` | Whole numbers | 4 bytes | -2.1B to 2.1B |
| `double` | Decimals | 8 bytes | 15-16 digits |
| `String` | Text | Varies | "Hello" |
| `boolean` | True/False | 1 bit | true/false |
| `char` | Single character | 2 bytes | 'A' |
| `long` | Very large numbers | 8 bytes | 19 digits |
| `float` | Small decimals | 4 bytes | 6-7 digits |

---

## ⚠️ Common Mistakes

### Mistake 1: Wrong Data Type
```java
❌ int price = 19.99;  // Error - 19.99 is not an int

✅ double price = 19.99;  // Correct
```

### Mistake 2: Quotes
```java
❌ String name = 'Ahad';     // Wrong - single quotes
❌ char grade = "A";          // Wrong - double quotes

✅ String name = "Ahad";      // Correct
✅ char grade = 'A';          // Correct
```

### Mistake 3: Variable Not Declared
```java
❌ System.out.println(age);  // Error - age not declared

✅ int age = 25;
   System.out.println(age);  // Correct
```

### Mistake 4: Reserved Words
```java
❌ int int = 5;     // Error - 'int' is reserved
❌ String class = "test";  // Error - 'class' is reserved

✅ int number = 5;  // Correct
✅ String className = "test";  // Correct
```

---

## 🎯 Key Takeaways

1. **Variables** store data with a name
2. **Data types** determine what kind of data a variable holds
3. **Primitive types** include: `int`, `double`, `String`, `boolean`, `char`
4. **Variable names** follow camelCase and can't be reserved words
5. **`final` keyword** makes a variable a constant
6. **Quotes matter**: Single `'` for char, Double `"` for String
7. **Type matters**: `int` for whole numbers, `double` for decimals

---

## 💡 Practice Tips

- Create variables and print them
- Change variable values and print again
- Try using different data types
- Experiment with invalid names (to see errors)
- Use descriptive variable names

---

## 🚀 What's Next?

Next, you'll learn about **Operators** - how to perform calculations and comparisons with your variables!

**Go to:** [03-Operators.md](03-Operators.md)

