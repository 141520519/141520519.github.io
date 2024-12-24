---
title: 4- Manipulation des données
tags:
  - sql
  - lecture
draft: false
subject: Sql
professor: Mahmoud Oussman
last_modified: 2024-12-24
---
### Suppression : Commande `DROP`
- **Syntaxe** : `DROP Table Nom_table;`
- **Exemple** : `DROP Table Emp;`

### Modification : Commande `ALTER`
- **Syntaxe** : `ALTER Table Nom_table Option`

#### Options de modification :

##### Colonne :
- **Ajouter une colonne** : `ADD Nom_att type attribut;`
- **Modifier une colonne** : `Modify Nom_att type attribut;`
- **Supprimer une colonne** : `DROP Column Nom_att;`

##### Contrainte d'intégrité :
- **Ajouter une contrainte** : `ADD Constraint definition constraint (PK, FK, UNIQUE, CHECK)`
- **Supprimer une contrainte** : `DROP Constraint Nom_conste`

- **Exemples** :
  - `ALTER table Emp DROP Constraint Emp_PK`
  - `ALTER table Emp ADD Constraint Emp_PK (Num_E, Nom_E)`
