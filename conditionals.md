# Conditionals

## Helpful Links

W3School [conditionals](https://www.w3schools.com/java/java_conditions.asp) and [switch](https://www.w3schools.com/java/java_switch.asp)

### Conditionals

A conditional is statement that will execute depending on the conditions. In programming, conditionals only deal with absolutes: true and false. Therefore, conditionals are linked with the primitive data type that deals with state: booleans.

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

An else statement will execute when the linked If statmment does not execute (this also includes elif statements).

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

An elif or else if statement executes if the previous if statement did not execute. This stament will preced the else statement but come after an if or another elif statement.

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

Another way to generate a boolean is to use the result of a >, < or = operator (there is also >= and <=).

```;ava
boolean myBool = 3>2;   // True
myBool = 3==2;          // False
```

> When comparing if two values equals, use == as a = represents setting a value.

> Do not use == to compare if strings equal in Java. There is a .equals function in the String class that should be used instead.

