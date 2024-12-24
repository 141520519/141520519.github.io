---
title: 2- Circle perimeter
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
import java.util.Scanner;

Scanner sc = new Scanner(System.in);

// Declare variables
double R, S, P;
final double pi = 3.14;

// Get radius input
System.out.println("Entrer le rayon du cercle");
R = sc.nextDouble();

// Calculate area and perimeter
S = pi * R * R;
P = 2 * pi * R;

// Print results
System.out.println("La surface du cercle = " + S);
System.out.println("La périmètre du cercle = " + P);

// Using Math class
S = Math.PI * Math.pow(R, 2);
P = 2 * Math.PI * R;
```