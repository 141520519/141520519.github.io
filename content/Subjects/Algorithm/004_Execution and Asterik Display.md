---
title: 4- Execution and Asterik Display
tags:
  - algo
  - code
  - exercise
draft: false
subject: Algorithm
professor: Mahmoud Oussman
last_modified: 2025-01-15
---
## Exercise1:
```Less
Entier i, j, N;
Debut
Ecrire("Int N:");
Lire(N);
pour i= 1 à N faire
	pour j= 1 à N-i + 1
	ecrire ("*");
	Fin j;
PAL;
Fin i
Fin;
```
## Run:
Enter N:
5
## Execution:
```Less
I= 5
	j= 1 à N(5)-i +1
		Ecrire("*");
PAL

I= 4
	j= 1 à N(4)-i +1
		Ecrire("*");
PAL

I= 3
	j= 1 à N(3)-i +1
		Ecrire("*");
PAL

I= 2
	j= 1 à N(2)-i +1
		Ecrire("*");
PAL

I= 2
	j= 1 à N(2)-i +1
		Ecrire("*");
PAL

I= 1
	j= 1 à N(1)-i +1
		Ecrire("*");
		Fin j
PAL

```

## Exercise 2:
## Run:
N= 5
```Less
S=0
Pour i= 1 à N faire
	S= S + i;

S=1
Pour i= 2 à N faire
	S= S + i;

S=2
Pour i= 3 à N faire
	S= S + i;

S=3
Pour i= 4 à N faire
	S= S + i;

S=4
Pour i= 5 à N faire
	S= S + i;

Fin i;

S= 15

Ecrire("Somme: ", S);
```
## Output:
Somme: 15

## Exercise 3:

## Code:

```Less
Debut
Entier N, j, i;
Ecrire("Entrer N: ");
Lire(N);
Pour i= 1 à N Faire
	Pour j= 1 à i faire
		Ecrire("*");
	Fin j
PAL;
Fin i
Fin
```
## Execution:
N= 5
```Less
i= 1
	pour j= 1 à i
PAL

i= 2
	pour j= 1 à i
PAL

i= 3
	pour j= 1 à i
PAL

i= 4
	pour j= 1 à i
PAL

i= 5
	pour j= 1 à i
PAL
```
## Output:
```Less
*
**
***
****
*****
```
## Exercise 4:

## Code:
```Less
Entier i, j, N, k
Debut
Ecrire("entrer N: ");
Lire(N);
Pour i= 1 à N faire
	Pour j= 1 à N-1
		Ecrire("Space")
	Fin j
	Pour k= 1 à 2*i-1 faire
		Ecrire("*");
	Fin k
Fin i;
PAL;
Fin
```
