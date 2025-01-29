---
title: 5- Loops
tags:
  - algo
  - code
draft: false
subject: Algorithm
professor: Mahmoud Oussman
last_modified: 2025-01-29
---
##### Pour (for)
```LESS
Algo boucle
Entier i, N, S;
Debut
Ecrire ("entrer N");
lire (N);
S=0;
pour i=1 à N faire
	S= S+i;
Fin i
Ecrire ("Somme = ", S);
Fin
```
--------
##### Tant-que (while)
```LESS
Algo boucle
Entier i, N, S;
Debut
Ecrire ("entrer N");
lire (N);
i=1;
S=0;
tant que (i <= N) faire
	S= S+i;
	i= i+1;
Fin tq
Ecrire ("la Somme = ", S);
Fin
```
-------
##### Repetez jusqu'a (do...while)
```less
Algo boucle
Entier i, N, S;
Debut
Ecrire ("entrer N");
lire (N);
i=1;
S=0;
Repeter
    S= S+i;
    i= i+1;
jusqu'a (i <= N)
Ecrire ("Somme = ", S);
Fin
```