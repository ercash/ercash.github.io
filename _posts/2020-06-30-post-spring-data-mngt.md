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

* `SQLException`
* `IOException`
* `ClassNotFoundException`
* `InvocationTargetException`

**Unchecked exceptions** are not checked at compile time. It means if your program is throwing an unchecked exception and even if you didn’t handle/declare that exception, the program won’t give a compilation error. 
All Unchecked exceptions are direct sub classes of **RuntimeException** class.

Here are the few **unchecked exception** classes:

* `NullPointerException`
* `ArrayIndexOutOfBoundsException`
* `ArithmeticException`
* `IllegalArgumentException`
* `NumberFormatException`

Source is [hier](https://beginnersbook.com/2013/04/java-checked-unchecked-exceptions-with-examples/ "Checked and unchecked exceptions in java with examples").

### Why does Spring prefer unchecked exceptions?

Spring prefers unchecked exception because this way it gives the developer possibility to choose to handle them or not - he is not enforced to handle them. To use Spring specific exceptions you must use Spring templates. `JdbcTemplate` takes care of transforming SQLExceptions to meaningful `DataAccessExceptions`, this is done using `SQLExceptionTranslators`.

### What is the data access exception hierarchy?

The data access exception hierarchy ... 
- [ ] <span style="color:red">TODO</span>

### How do you configure a DataSource in Spring?
- [ ] <span style="color:red">TODO</span>

#### Which bean is very useful for delevopment/test databases?
Embedded!
- [ ] <span style="color:red">TODO</span>

### What is the Template design pattern and what is the JDBC template?
- [ ] <span style="color:red">TODO</span>

### What is Callback?
- [ ] <span style="color:red">TODO</span>

#### What are the three `JdbcTemplate` callback interfaces that can be used with queries?
- [ ] <span style="color:red">TODO</span>

#### What is each used for?
- [ ] <span style="color:red">TODO</span>

> You would not have to remember the interface names in the exam, but you should know what they do if you see them in a code sample.

### Can you execute a plain SQL statement with the JDBC template?
- [ ] <span style="color:red">TODO</span>

### When does the JDBC template acquire (and release) a connection, for every method called or once per template? 
- [ ] <span style="color:red">TODO</span>

#### Why?
- [ ] <span style="color:red">TODO</span>

### How does the `JdcbTemplate` support generic queries? 
- [ ] <span style="color:red">TODO</span>

#### How does it return objects and lists/maps of objects?
- [ ] <span style="color:red">TODO</span>

---

