---
title: 7- Homework 1 Solution
tags:
  - sql
  - exercise
draft: false
subject: Sql
professor: Mahmoud Oussman
last_modified: 2025-1-26
---
### Exercise 1:
1. 
```sql
SELECT Montant AS HT, (Montant + (Montant * TVA)/100) AS TTC FROM Factures;
```
2. 
```SQL
SELECT Montant, date_f FROM Factures WHERE nom_cl= Dupont;
```
3. 
```SQL
SELECT Sum(Montant), nom_cl FROM Factures GROUP BY nom_cl
```
4. 
```SQL
SELECT nom_cl, Avg(Montant) FROM Factures HAVING Count(nom_cl) > 1;
```
5. 
```SQL
SELECT numero, montant FROM Factures WHERE nom_cl= Dupont OR nom_cl= Durand;
```

### Exercise 2:

```SQL
SELECT Telephone FROM Factures, Clients WHERE Factures.nom_cl= Clients.nom_cl AND Clients.ville= Toulouse
```