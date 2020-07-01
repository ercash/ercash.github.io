---
title: "Data Management: JDBC, Transactions"
date: 2020-06-30T16:00:00-00:00
categories:
  - spring-certification
tags:
  - spring
  - certification
  - jdbc
  - transaction
toc: true
toc_label: "Topic: Spring Data Management"
---

Spring Data Management: JDBC (4%), Transactions (8%)

## Whats is the difference between checked and unchecked exceptions?

The **main difference between checked and unchecked exception** is that the **checked** exceptions are checked at <span style="color:red">**compile-time**</span> while **unchecked** exceptions are checked at <span style="color:red">**runtime**</span>.

**Checked exceptions** are checked at compile-time. It means if a method is throwing a checked exception then it should handle the exception using **try-catch block** or it should declare the exception using **throws keyword**, otherwise the program will give a compilation error.

Here are the few other **Checked Exceptions**:

* SQLException
* IOException
* ClassNotFoundException
* InvocationTargetException

**Unchecked exceptions** are not checked at compile time. It means if your program is throwing an unchecked exception and even if you didn’t handle/declare that exception, the program won’t give a compilation error. 
All Unchecked exceptions are direct sub classes of **RuntimeException** class.

Here are the few **unchecked exception** classes:

* NullPointerException
* ArrayIndexOutOfBoundsException
* ArithmeticException
* IllegalArgumentException
* NumberFormatException

Source is [hier](https://beginnersbook.com/2013/04/java-checked-unchecked-exceptions-with-examples/ "Checked and unchecked exceptions in java with examples")

### Why does Spring prefer unchecked exceptions?

TODO

### What is the data access exception hierarchy?

TODO

---

