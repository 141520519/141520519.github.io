---
title: 3- Salary Calculation and Color Display
tags:
  - algo
  - code
  - exercise
draft: false
subject: Algorithm
professor: Mahmoud Oussman
last_modified: 2024-12-23
---
## Exercice 1 : Calcul du salaire net
```less
Algorithm Tax
Begin
    Character name;
    Integer salary;
    Reel netSalary;
    Begin
        Write("Your name");
        Read(name);
        Write("Enter salary");
        Read(salary);
        if (salary < 500)
            Write("error");
        else if (salary > 500) and (salary < 1000)
            netSalary = salary - (salary * 10 / 100);
        else if (salary >= 1000) and (salary < 5000)
            netSalary = salary - (salary * 15 / 100);
        else if (salary >= 5000)
            netSalary = salary - (salary * 20 / 100)
        else
            Write("Net salary =", netSalary);
        Endif
    End
```

## Exercice 2 : Affichage d'une couleur
```
Algorithm Color
Integer number;
Begin
    Write("Enter number");
    Read(number)
    Case(number)
        Case 1: Write("Red");
        Case 2: Write("White");
        Case 3: Write("Yellow");
        Case 4: Write("Black");
        Default: Write("Error");
    Endcase
End
```