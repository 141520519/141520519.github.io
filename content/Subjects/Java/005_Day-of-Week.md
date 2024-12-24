---
title: 5- Day of Week
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
   int nbj;
   Scanner sc = new Scanner(System.in);
   
   System.out.println("entrez le nombre du jour");
   nbj = sc.nextInt();

   if (nbj == 1) {
       System.out.println("lundi");
   }
   else if (nbj == 2) {
       System.out.println("mardi");
   }  
   else if (nbj == 3) {
       System.out.println("mercredi");
   }
   else if (nbj == 4) {
       System.out.println("mercredi jeudi");
   }
   else if (nbj == 5) {
       System.out.println("vendredi");
   }
   else if (nbj == 6) {
       System.out.println("samedi");
   }
   else if (nbj == 7) {
       System.out.println("dimanche");
   }
}
```