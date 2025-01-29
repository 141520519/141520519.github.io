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

| numéro | date_f     | montant | nom_cl   | tva  |
| :----- | :---------- | :------ | :-------- | :--- |
| 1      | 04/04/2000  | 1200    | Dupont    | 19.6 |
| 2      | 11/10/2000  | 500     | Durand    | 5.5  |
| 3      | 12/11/2000  | 800     | Dupont    | 19.6 |
| 4      | 31/12/2000  | 2000    | Dubois    | 5.5  |
| 5      | 2/01/2001   | 900     | Ducarton  | 19.6 |
| 6      | 12/02/2001  | 500     | Dubois    | 5.5  |

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

| nom_cl   | ville    | téléphone | age |
| :------- | :------- | :--------- | :-- |
| Dupont   | toulouse | 1          | 18  |
| Durand   | tarbes   | 2          | 21  |
| Dubois   | pau      | 3          | 41  |
| Ducarton | tarbes   | 4          | 65  |

```SQL
-- Q1:
Select telephone from factures, Client
where factures.nom_cl = Client.nom_cl
And ville = 'toulouse';

-- Q2:
Select (montant + (montant * TVA) / 100) As chiffre_d_affaire
from factures f, client C
Where f.nom_cl = C.nom_cl
AND C.ville = 'toulouse';

-- Q3:
Select AVG(montant)
from factures F, client C
where C.nom_cl = f.nom_cl
Group by ville;

-- Q4:
Select Nom_cl from client
Where ville = 'pau' OR ville = 'toulouse' OR ville = 'tarbes';

-- Q5:
update client set ville = 'Albi' where nom_cl = 'Dupont';

-- Q6:
delete from client
where nom_cl = 'Dubois';
```
