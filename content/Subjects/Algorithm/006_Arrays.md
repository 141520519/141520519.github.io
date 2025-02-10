---
title: 6- Arrays
tags:
  - algo
  - code
  - exercise
draft: false
subject: Algorithm
professor: Mahmoud Oussman
last_modified: 2025-02-5
---
```LESS
Algo tableau voyelle / Non voyelle

Caractère t [N];

Entier i, N, V, NV;

debut

  Ecrire ("entrer le nombre des élément du tableau ");

  lire (N);

  pour i = 1 à N faire
    lire (t[i]); 
  fin pour

  V = 0;  // Initialize vowel count
  NV = 0; // Initialize non-vowel count

  pour i = 1 à N faire
    Si (T[i] = 'a' ou T[i] = 'e' ou T[i] = 'i' ou T[i] = 'o' ou T[i] = 'u') alors
      V = V + 1;
    Sinon  // It's a consonant or other character
      NV = NV + 1;
    fin si
  fin pour

  Ecrire ("nb voyelle = ", V); // Output vowel count
  Ecrire ("nb Non voyelle = ", NV); // Output non-vowel count

fin
```