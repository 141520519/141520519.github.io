---
title: 6- Queries
tags:
  - sql
  - lecture
draft: false
subject: Sql
professor: Mahmoud Oussman
last_modified: 2025-01-26
---
## Achat:

| ID  | Client | Tarif | Date      |
| --- | ------ | ----- | --------- |
| 1   | Pierre | 102   | 1/1/2000  |
| 2   | Simon  | 47    | 5/1/2000  |
| 3   | Marie  | 18    | 10/2/2000 |
| 4   | Marie  | 20    | 15/3/2000 |
| 5   | Pierre | 16    | 1/4/2000  |
## Between:
- Syntax: 
```sql
SELECT * FROM Table
WHERE attribute between 'Value 1' AND 'Value 2';
```
Example: 
```sql
SELECT Client From Achat
WHERE date between '5/1/2000' AND '15/3/2000';
```
## Integrity Function:
- Sum()
- Avg()
- Max()
- Min()
- Count()
- Syntax:
```sql
SELECT Name Function (attribute) FROM Table;
```
- Example:
```SQL
SELECT Max(Tarif) FROM Achat;
SELECT Min(Tarif) FROM Achat;
SELECT Sum(Tarif) FROM Achat;
SELECT Avg(Tarif) FROM Achat;
Select Count(Client) FROM Achat;
SELECT Count(Distinct Client) FROM Achat;
```
## Change virtual table's name (Results table):
```SQL
SELECT Max(Tarif) As Maximum FROM Achat;
```
## Order by:
- Syntax
```SQL
SELECT * FROM Table
WHERE HAVING ORDER BY Asc/Desc;
SELECT Client FROM Achat
ORDER BY Tarif Asc;
```
## Having:
- Syntax
```SQL
SELECT * FROM Table HAVING Function ><=;
```
## Group by:
```SQL
SELECT Client, Sum(Tarif) FROM Achat
GROUP BY Client;
```

| Client | Sum(Tarif) |
| ------ | ---------- |
| Pierre | 118        |
| Simon  | 47         |
| Marie  | 38         |

```SQL
SELECT Client, Count(Tarif) FROM Achat
GROUP BY Client;
```