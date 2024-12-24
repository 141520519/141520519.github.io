---
title: 3- Calcul Combinatoire
tags:
  - statistics
  - lecture
  - exercise
  - latex
draft: false
subject: Statistics
professor: Amina Dankar
last_modified: 2024-12-24
---
# 1. Factorielle:
$$
n! = 1 \times 2 \times \cdots \times (n-1) \times n
$$
- Exemple:
$$
3! = 1 \times 2 \times 3 = 6
$$
$$
5! = 1 \times 2 \times 3 \times 4 \times 5 = 120
$$
$$
\frac{8!}{6!} = \frac{1 \times 2 \times \cdots \times 6 \times 7 \times 8}{1 \times 2 \times \cdots \times 6} = 56
$$
$$
\frac{10!}{7!} = \frac{10 \times 9 \times 8 \times 7 \cdots \times 1}{7 \times \cdots \times 1} = 720
$$
- Note: \( 0! = 1 \)

# 2. P-listes:
![[Statistics-IMG-0012.jpg]]
- Dans le cas où l'ordre est important et la répétition est permise, le nombre de tirages est:
$$
n^p
$$
- Exemple: Soit \( E = \{a, b, c\} \), \( n = 3 \).
Les 2-listes d'éléments de \( E \): 
- (a, a)
- (a, b)
- (a, c)
- (b, a)
- (b, a)
- (b, b)

Le nombre total est: \( 3^2 = 9 \).

# 3. Arrangements sans répétition:
- Dans ce cas, l'ordre est important mais il n'y a pas de répétition.
Le nombre de tirages est:
$$
A^p_n = \frac{n!}{(n-p)!}
$$
- Exemple: Soit \( E = \{a, b, c\} \).
Les arrangements sans répétition d'ordre 2 de \( E \):
- (a, b)
- (a, c)
- (b, a)
- (b, c)
- (c, a)
- (c, b)

Le nombre total est:
$$
A^2_3 = \frac{3!}{(3-2)!} = \frac{1 \times 2 \times 3}{1!} = 6
$$

# 4. Permutation:
- Arrangement sans répétition avec \( n = p \).
Le nombre de permutations est:
$$
A^n_n = \frac{n!}{(n-n)!} = \frac{n!}{0!} = \frac{n!}{1} = n!
$$
- Exemple: Soit \( E = \{a, b, c\} \).
Les permutations de \( E \) sont:
- (a, b, c)
- (a, c, b)
- (b, a, c)
- (b, c, a)
- (c, a, b)
- (c, b, a)

Le nombre total est \( 3! = 1 \times 2 \times 3 = 6 \).

- Propriété:
$$
A^1_n = n
$$

# 5. Combinaison:
- Sans ordre et sans répétition.
Le nombre de combinaisons est:
$$
C^p_n = \frac{n!}{p!(n-p)!}
$$
- Exemple: Soit \( E = \{a, b, c\} \).
Les combinaisons d'ordre 2 de \( E \):
- {a, b}
- {a, c}
- {b, c}

Le nombre total est:
$$
C^2_3 = \frac{3!}{2!(3-2)!} = \frac{1 \times 2 \times 3}{2 \times 1 \times 1} = 3
$$
