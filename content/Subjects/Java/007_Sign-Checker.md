---
title: 7- Sign Checker
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

public class ProductSign {

    public static void main(String[] args) {

        int nb1, nb2;

        Scanner sc = new Scanner(System.in);

        System.out.print("entrer le 1er nombre: "); // Corrected text

        nb1 = sc.nextInt();

        System.out.print("entrer le 2e nombre: "); // Corrected text

        nb2 = sc.nextInt();

        if ((nb1 > 0 && nb2 > 0) || (nb1 < 0 && nb2 < 0)) {
            System.out.println("Le produit est positif.");
        } else if (nb1 == 0 || nb2 == 0) {
            System.out.println("Le produit est nul.");
        } else {
            System.out.println("Le produit est negatif.");
        }
    }
}
```