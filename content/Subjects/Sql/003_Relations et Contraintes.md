---
title: 3- Relations et Contraintes
tags:
  - sql
  - lecture
  - exercise
  - code
draft: false
subject: Sql
professor: Mahmoud Oussman
last_modified: 2024-12-24
---
# Q1) Créer tableau Emp

```sql
CREATE TABLE Emp (
    NumE NUMBER(3),
    NomE VARCHAR2(20),
    Fonction VARCHAR2(20),
    Embauche DATE,
    Salaire NUMBER(5),
    Comm NUMBER(3),
    NumD NUMBER(1),
    CONSTRAINT Emp_pk PRIMARY KEY (NumE),
    CONSTRAINT Emp_fk FOREIGN KEY (NumD) REFERENCES Dept(NumD),
    CONSTRAINT Emp_check CHECK (Salaire > 0)
);
````

# Q2) Clé primaire et clé étrangère

- **Clé primaire** : `NumE` (le numéro d'employé)
- **Clé étrangère** : `NumD` (le numéro du département), qui référence `NumD` dans la table `Dept`

# Q3) Contraintes supplémentaires

- Lieu dans la table `Dept` doit être l'un des suivants : Dallas, Boston, ou Miami.
- Salaire doit toujours être supérieur à zéro.

# Q4) Insérer les valeurs dans le tableau Dept

```sql
INSERT INTO Dept VALUES (1, 'Commerce', 'Dallas');
INSERT INTO Dept VALUES (2, 'Droit', 'Boston');
```