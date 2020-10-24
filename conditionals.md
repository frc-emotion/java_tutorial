# Conditionals

## Helpful Links

W3School [conditionals](https://www.w3schools.com/java/java_conditions.asp) and [switch](https://www.w3schools.com/java/java_switch.asp)

### Conditionals

A conditional is statement that will execute depending on the conditions. In programming, conditionals only deal with absolutes: true and false. Therefore, conditionals are linked with the primitive data type that deals with state: booleans.

```java
/* Format
/ if/elif (conditional) {
/   code block executed
/}

if (true) {
  System.out.Println("true");
}
```

#### If

An if statement will execute with the given condition is true.

```java
boolean myBool = true;

if (myBool) {
  System.out.println("myBool is true"); 
}

// console : "myBool is true"
```

#### Else

An else statement will execute when the linked If statmment does not execute (this also includes elif statements). There can only be one else statement in each chain.

```java
boolean myBool = false;

if (myBool) {
  System.out.println("myBool is true
} else {
  System.out.println("myBool is false);
}

// console : "myBool is false"
```
#### Elif

An elif or else if statement executes if the previous if statement did not execute and the conditional is true. This stament will preced the else statement but come after an if or another elif statement.

```java
boolean myBool = false;

if (myBool) {
  System.out.println("myBool is true
} elif (!myBool) {
  System.out.println("myBool is false);
}

// console : "myBool is false" 
```
> The ! operetor acts as the not in other languages. This reverses the boolean it acts on.

### Conditional Chain

The nature of conditionals allows it to chain together in this format

> If<br>
Elif<br>
Elif<br>
...<br>
Else

This common format occurs in code that controls the flow of operation and handles errors. For example, in the rbotos code, we parse the controller inputs of what buttons are pressed using a conditional chain.

```java
// A code snippet from the drivetrain main run statement

if (Robot.driverController.getAButtonPressed()) {
    invert = !invert;
}

if (Robot.driverController.getBButton()) {
    align();
} else {
    runTankDrive();
    reset();
}
```
### Mathematic Conditionals

Another way to generate a boolean is to use the result of a comparison operator (>, <, <=, >=, and ==) .

```java
boolean myBool = 3>2;   // True
myBool = 3==2;          // False
```

> When comparing if two values equals, use == as a = is used to set a value to a variable.

> Do not use == to compare if strings equal in Java. There is a .equals function in the String class that should be used instead.

### Functional Conditionals

In a later article, we will cover functions which can returns data that can be stored in a variable or used immediately. However, we will cover a situation where a function returns a boolean which can be directly used in place of a boolean variable.

```java
String myString = "same string";
if (myString.equals("same string") {
  System.out.println("the string is the same as myString");
}
```

> a String object has a function called .equals(String) which returns a boolean depending on whether the passed string is the same.

### Switch Statment

A switch statement is provided in Java and other languages to simplify a common use of if/elif chains where you compare an input to different values. In a switch statement, the 


