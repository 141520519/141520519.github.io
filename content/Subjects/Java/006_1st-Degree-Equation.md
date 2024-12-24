---
title: 6- 1st Degree Equation
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

public class EquationSolver {

    public static void main(String[] args) {

        double a, b, x;

        Scanner sc = new Scanner(System.in);

        System.out.println("entrer la valeur de a");

        a = sc.nextDouble();

        System.out.println("entrer la valeur de b");

        b = sc.nextDouble();

        if (a == 0) {
            if (b == 0) {
                System.out.println("infinité de solution");
            } else {
                System.out.println("solution impossible");
            }
        } else {
            System.out.println("x=" + (-b / a));
        }
    }
}
```