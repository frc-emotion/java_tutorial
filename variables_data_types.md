# Variables and Data Types

## Helpful Links
W3school [variables](https://www.w3schools.com/java/java_variables.asp) and [datatypes](https://www.w3schools.com/java/java_data_types.asp)

###Variables

**What is a Variable?**

A variable stores a value for future usage.

**Components of a Variable**

A variable has two main components, the name and the value. The name allows you to access the value later for reading and writing a value.

```java
int myVar = 8;
```

**Declaring a Variable**

As shown in the previous example, you can declare a variable through the syntax.

```java
char myVar = 'c';
```

> The data type is specified before the name. We will discuss the meaning behind this later.

You can also declare a variable without passing a value. However, you must assign a value before reading from it.

```java
boolean myVar;
```

**Assigning a Value to a Declared Variable**

To assign a value to a declared variable, you use the syntax.

```java
// Declaration
int myVar = 10;

// Assignment
myVar = 15;
```

> The data type is not needed when assigning a value to a variable.

**Reading the Value**

To read the value of a variable, you use the name of the variable instead of a literal value such as the integer 1 or the string “hello world”.

```java
int myVar = 15;

System.out.println(myVar); // outputs "15" in the console
```


> This name can be used instead of a literal or an explicitly typed value.

