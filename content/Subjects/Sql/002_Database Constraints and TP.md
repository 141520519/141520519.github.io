---
title: 2- Database Constraints and TP
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
## Integral Constraints

### Primary Key
- **Format**: `Constraint Name.Const Primary Key (att)`
- **Example**:  
  `Constraint Emp.PK primary key (Nom-E)`

### Foreign Key
- **Format**: `Constraint Name.Const Foreign Key (att) references Nom-table (att)`
- **Example**:  
  `Constraint Emp.FK foreign key (Num_D) references Dep (Num D)`

### Check
- **Format**: `Constraint Nom-Const check (att condition)`
- **Example**:  
  `Constraint Ville-D.check Check ville-D in (Tripoli, Beirut)`

### Unique
- **Format**: `Constraint Nom-Const Unique (att)`
- **Example**:  
  `Constraint Nom.Un Unique (Nom-D)`

---

## Practical Example

### Create Table: `Emp`
```sql
Create Table Emp ( 
    Num-E number (2),
    Nom-E varchar2 (10),
    Salaire-E number (4),
    Num-D number (2),
    Constraint Emp.PK primary key (Nom-E),
    Constraint Emp.FK foreign key (Num_D) references Dep (Num D),
    Constraint Sal.check Check (Salaire-E > 400)
);
````

### Create Table: `Dep`

```sql
Create Table Dep (
    Num-D number (1),
    Nom-D varchar2 (20),
    Ville-D varchar2 (10),
    Constraint Dep.PK primary Key (Num-D),
    Constraint Nom.Un Unique (Nom-D),
    Constraint Ville-D.check check ville-D in (Tripoli, Beirut)
);
```