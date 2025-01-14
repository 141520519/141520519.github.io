---
title: 5- Données Relationnelles
tags:
  - sql
  - lecture
  - exercise
draft: false
subject: Sql
professor: Mahmoud Oussman
last_modified: 2025-1-14
---
# Emp:

| Num_E | Nom_E | Sal_E | Num_D |
| ----- | ----- | ----- | ----- |
| 1     | A     | 700   | 1     |
| 2     | B     | 1300  | 2     |
| 3     | C     | 800   | 1     |

# Dep:

| Num_D | Nom_D       | Ville   |
| ----- | ----------- | ------- |
| 1     | Vente       | Beirut  |
| 2     | Fabrication | Tripoli |

## Integration des données:

- SQL
- Algèbre relationnelle

## En SQL:

### Syntaxe:
```sql
Select Nom_attribut From table;
```
Ex:
```SQL
Select Sal From Emp;
```
1) Donnez tous les informations du table Emp
	
```sql
Select Num_E, Nom_E, Sal_E, Num_D From Emp
Select * From Emp;
```
2) Donnez les noms et salaires des employez
```sql
Select Nom_E, Sal_E From Emp;
```
3) Donnez tous les informations du tableau Dep;

```sql
Select * From Def;
```
4) Donnez les noms et les villes des departement

```sql
Select Nom_D, Ville From Def;
```
5) Donnez les noms des employer qui travaille dans departement fabrication

```sql
Select Nom_E From Emp, Dep
Where Emp.Num_D = Rep.Num_D
AND Nom_D = Fabrication;
```
6) Donnez les noms des employees dont les salaires plus grand que 900

```sql
Select Nom_E From Emp
Where Sal_E > 900;
```

7) Donnez les noms du departement qui trouve a tripoli

```sql
Select Nom_D From Dep
Where Ville = Tripoli;
```
8) Donnez les noms et les salaires des employees qui travaille a Beirut et son salaire plus petit que 1000

```Sql
Select Nom_E, Sal_E From Emp, Dep
Where Emp.Num_D = Dep.Num_D
AND Ville = Beirut
AND Sal_E < 1000;
```