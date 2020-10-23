# Variables and Data Types

## Helpful Links
W3school [variables](https://www.w3schools.com/java/java_variables.asp) and [datatypes](https://www.w3schools.com/java/java_data_types.asp)

### Variables

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

#### Conclusion

A variable is a component in programming languages that allows a programmer to refrence data that was previously stored. Later, we will explore how a variable can be used to implement more complex ideas.

```java
// Declaration

// Data type / Name = Value
float myFloat = 0.3;

// Data type / Name
int myInt;

// Assignment
myFloat = 0.6;
myInt = 3;

// Reading
System.out.println(myInt);
```

### Data Types

Each variable has a explict or implied data type. In Java, a statistically typed language, each variable must be explicity given a data type during declaration, regardless if a value is provided.

```java
// int is the data type of myInt
int myInt;

```

> After introducing the concept of classes, we will define data types differently. In Python, a dynamic language, the data type is implied from the value and the value's type can change during runtime.

#### Primitive Data Types

There are four primitive data types: integer, float, character, and boolean. These data types are implemented natively in the language and are expanded upon by higher data types.

> There are sub categories within integer and float that are exponsed in certain languages that allows the programmer to explicitly control the bit size of the variable.

**Integer**

An integer is a whole number that can be positive or negative (zero is also an integer).

```java
1 -15 3002
```

**Float**

A float is a number that contains decimal places.

```java
1.32 -35.351 234234.00002
```

**Character**

A character in Java is a unicode character enclosed by single quotes (').

```java
'b' '\b' '"'
```

> Another popular method of storing characters is ASCII

**Boolean**

A boolean stores a true or false statement. This data type is primarily used to store the output of conditionals.

```java
true false
```
#### Implementation in Java

Compared to class defined data types, primitive data types in Java are lowercased.

```java
int myInt;
float myFloat;
char myChar;
boolean myBool;
```

#### What about String?

The first clue on the classification of String is its capitalization. Later on, we will explore the true meaning behind a capitalized data type. But for now, we will view all data types that are capitalized as not primitive.

**Why is String not Considered a Primitive?**

A String is not considered a primitive as it is a collection of characters, a primitive data type. This separation between primitive and non primitive will be important when defining later concepts.

```java
String myString;
```

#### Conclusion

A data type defines what a variable can store. In Java, the data type of a variable **cannot** change during runtime, when the program is executed, such that a different data type can be placed in a data type specified for something else.

```java
// This does not work
String myString = "hello_world";
myString = 3;
```
In Java, there are four primitive data types: integer, float, character, and boolean. These data types are implemented by the language and are lowercased to be differentiated from non primitive data types.

## Optional


### Static vs Dynamic Languages
As I mentioned before, Java data types are static, such that they cannot change during runtime. Therefore, we call Java a statistically typed language. Another type of language exists called dynamically typed languages that allows variables to change their type during runtime. For example, Python allows you to set a variable originally holding an integer to now having the value of a string.

```python
# This does not work in Java
myInt = 10
myInt = "hello_world"
```

This ability to change data types during runtime can lead to type errors where a variable's data type might not match the expected result. For example, a variable previously set to an integer that was changed to a string cannot be used in arithmetic.

```python
# Do not worry about this function. This is just an example of a case where you expect an integer input.
def add_one(addend):
  return addend + 1

myInt = "hello_world"
print(add_one(myInt)) # Will raise a TypeError when trying to add a string to an Int
```

We will not discuss the benefits and negatives of this design choice in this article as the scenarios extend beyond the scope of our lesson. However, with enough intrest, I may create an article on Dynamic vs Static languages later.
