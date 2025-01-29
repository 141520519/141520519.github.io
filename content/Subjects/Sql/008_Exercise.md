---
title: 8- Exercise
tags:
  - sql
  - exercise
draft: false
subject: Sql
professor: Mahmoud Oussman
last_modified: 2025-1-29
---
### Exercise 1:
Q1. (Not answered)
Q2. 
```SQL
SELECT Poste FROM EMP WHERE sal >=1000 ORDER BY Poste DESC GROUP BY Poste;
```
Q3.
```SQL
SELECT noemp, Poste FROM EMP, Dept WHERE nodept= 10;
```
Q4. 
```SQL
SELECT noemp FROM EMP, PROJET WHERE p.noproj= e.noproj AND p.nomproj= 'Alpha'
```
Q5.
```SQL
SELECT noemp FROM EMP, DEPT WHERE p.nodept = e.nodept AND nomdept= 'recherche';
```
Q6.
```SQL
SELECT noemp FROM EMP, DEPT, PROJET WHERE e.nodept= d.nodept AND e.noproj= p.noproj AND nomdept= 'fabrication' AND projet= 'alpha';
```
Q7.
```SQL
SELECT nomemp, Poste, sal FROM EMP, DEP WHERE e.nodept= d.nodept AND nomdept= 'Ventes';
```
Q8.
```SQL
SELECT nomemp, poste FROM EMP WHERE Poste IN (SELECT Poste FROM Emp WHERE nomemp='Biraud');
```