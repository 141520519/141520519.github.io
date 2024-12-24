---
title: 4- Max Number
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

public class MaxNumber {
    public static void main(String[] args) {
        // Declare variables
        int nb1, nb2, max;
        Scanner sc = new Scanner(System.in);
            // Get first number
            System.out.println("Entrer un nb entier");
            nb1 = sc.nextInt();
            
            // Get second number
            System.out.println("Entrer un autre nb");
            nb2 = sc.nextInt();
            
            // Find maximum
            if (nb1 > nb2) {
                max = nb1;
            }
            else {
                max = nb2;
            }
            
            // Print result
            System.out.println("Le max entre " + nb1 + " et " + nb2 + " est " + max);
            
            System.out.println("Error: Please enter valid integers");    
}
```