---
title: 1- Création et Manipulation des Tables
tags:
  - sql
  - lecture
  - exercise
  - code
  - table
draft: false
subject: Sql
professor: Mahmoud Oussman
last_modified: 2024-12-24
---
## 1. Création de tableau

### Attributs
- **Nom**
- **Type**:
  - **Numero**: `Number`
  - **Caractère**: `VarChar21`
- **Size**

### Syntaxe de Création du Tableau
```sql
CREATE TABLE Table_Name (
    Attribut1 Type(Size),
    Attribut2 Type(Size),
    Attribut3 Type(Size)
);
```
#### Exemple 1

```sql
CREATE TABLE Elève (
    NumeroE Number(2),
    NomE Varchar2(20),
    Age Number(2)
);
```

#### Exemple 2

```sql
CREATE TABLE Produit (
    ID_P Number(5),
    NomP Varchar2(20),
    Prix_P Number(8)
);
```

---

## 2. Insertion des informations dans les tableaux

### Syntaxe

```sql
INSERT INTO Table_Name VALUES (ValeurAtt1, ValeurAtt2, ValeurAtt3);
```

#### Exemple

```sql
INSERT INTO Produit VALUES (1, 'A', 5000000);
INSERT INTO Produit VALUES (2, 'B', 2000000);
```

### Exemple de Table Résultante

|ID_P|Nom_P|Prix_P|
|---|---|---|
|1|A|5000000|
|2|B|2000000|

---

## 3. Contraintes

### Types de Contraintes

1. **Primary Key**
2. **Secondary Key**
3. **Check**:
    - **Number**: `<`, `>`, `=`
    - **CharVar**: `LIKE`, `IN`
4. **Unique**

---

## 4. Interrogation des Données

### 1. SQL

Utilisez des commandes SQL pour interroger les données insérées.

### 2. Algèbre Relationnelle

Manipulation des données à l'aide des expressions d'algèbre relationnelle.

---

## Exemple de Relation entre deux Tables

### Table 1

|Code_P|Nom_P|ID_P|
|---|---|---|
|961|LIBAN|2|
|965|KSA|1|

### Table 2

|ID_P|Nom_P|Code_P|
|---|---|---|
|1|A|965|
|2|B|961|