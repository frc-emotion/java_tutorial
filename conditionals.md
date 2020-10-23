# Conditionals

## Helpful Links

W3School [conditionals](https://www.w3schools.com/java/java_conditions.asp) and [switch](https://www.w3schools.com/java/java_switch.asp)

### Conditionals

A conditional is statement that will execute depending on the conditions. In programming, conditionals only deal with absolutes: true and false. Therefore, conditionals are linked with the primitive data type that deals with state: booleans.

#### If

An If statement will execute with the given condition is true.

```java
boolean myBool = true;

if (myBool) {
  System.out.println("myBool is true"); 
}

// console : "myBool is true"
```

#### Else

An Else statement will execute when the linked If statmment does not execute (thisalso includes elif statements).

```java
boolean myBool = false;

if (myBool) {
  System.out.println("myBool is true
} else {
  System.out.println("myBool is false);
}

// console : "myBool is false"
```
