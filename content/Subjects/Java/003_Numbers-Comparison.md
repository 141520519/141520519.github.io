---
title: 3- Numbers Comparison
tags:
  - java
  - code
  - exercise
draft: false
subject: Java
professor: Ziad Hoblos
last_modified: 2024-12-23
---
```java
public static void main(String[] args) {
    // Declare variables
    int x, y;
    Scanner sc = new Scanner(System.in);
    
    // Get first number
    System.out.println("Entrer un nb entier x = ");
    x = sc.nextInt();
    
    // Get second number
    System.out.println("Entrer un autre nb y = ");
    y = sc.nextInt();
    
    // Compare numbers
    if (x > y) {
        System.out.println(x + " plus grand que " + y);
    }
    else if (x < y) {
        System.out.println(x + " plus petit que " + y);
    }
    else {
        System.out.println(x + " et " + y + " sont égale");
    }
}
```
