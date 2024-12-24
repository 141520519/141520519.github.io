---
title: 1- Numbers Sum
tags:
  - java
  - code
draft: false
subject: Java
professor: Ziad Hoblos
last_modified: 2024-12-23
---
```java
import java.util.Scanner;

String fname, lname;
Scanner sc = new Scanner(System.in);

System.out.println("Enter your first name:");
fname = sc.next();

System.out.println("Enter your last name:");
lname = sc.next();

System.out.println(fname + lname);

int nb1, nb2, S = 0;

System.out.println("Enter the 1st int number");
Scanner sc = new Scanner(System.in);
nb1 = sc.nextInt();

System.out.println("Enter the 2nd int number");
nb2 = sc.nextInt();
S = nb1 + nb2;

System.out.println("Total= " + S);
System.out.println(nb1 + "+" + nb2 + "=" + S);

S = (double)nb1/nb2;
```