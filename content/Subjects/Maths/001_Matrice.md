---
title: 1- Matrice
tags:
  - lecture
  - maths
  - latex
draft: false
subject: Maths
professor: 
last_modified: 2025-01-29
---
==Nb de ligne n(<-->)=== M_(n;m)==Nb de colonne m==
### Somme de deux matrices
Il faut que les 2 matrices: meme nb de ligne; meme nb de colonne.
$$
A = \begin{pmatrix}
1 & 2 & -3 \\
2 & 0 & 4
\end{pmatrix}
$$
$$
B = \begin{pmatrix}
5 & 6 & 10 \\
-1 & -2 & 0
\end{pmatrix}
$$
$$
A_{2,3}
$$
$$
A + B = C_{2;3} = \begin{pmatrix}
1 + 5 & 2 + 6 & -3 + 10 \\
2 + (-1) & 0 + (-2) & 4 + 0
\end{pmatrix} = \begin{pmatrix}
6 & 8 & 7 \\
1 & -2 & 4
\end{pmatrix}
$$
### Produit par une constant
$$
3A = \begin{pmatrix}
3(1) & 3(2) & 3(-3) \\
3(2) & 3(0) & 3(4)
\end{pmatrix} = \begin{pmatrix}
3 & 6 & -9 \\
6 & 0 & 12
\end{pmatrix}
$$
### Combinaison
$$
3A = \begin{pmatrix}
3 \cdot 1 & 3 \cdot 2 & 3 \cdot (-3) \\
3 \cdot 2 & 3 \cdot 0 & 3 \cdot 4
\end{pmatrix} = \begin{pmatrix}
3 & 6 & -9 \\
6 & 0 & 12
\end{pmatrix}
$$
$$
2B = \begin{pmatrix}
2 \cdot 5 & 2 \cdot 6 & 2 \cdot 10 \\
2 \cdot (-1) & 2 \cdot (-2) & 2 \cdot 0
\end{pmatrix} = \begin{pmatrix}
10 & 12 & 20 \\
-2 & -4 & 0
\end{pmatrix}
$$
$$
3A - 2B = \begin{pmatrix}
3 & 6 & -9 \\
6 & 0 & 12
\end{pmatrix} - \begin{pmatrix}
10 & 12 & 20 \\
-2 & -4 & 0
\end{pmatrix}
$$
$$
= \begin{pmatrix}
7 & -6 & -29 \\
8 & 4 & 12
\end{pmatrix}
$$

---
$$
C = \begin{pmatrix}
1 & -2 & 3 \\
-1 & 2 & 1 \\
0 & -1 & 2
\end{pmatrix}
$$
$$
D = \begin{pmatrix}
-1 & 2 & -2 \\
-1 & 3 & -3 \\
-1 & -1 & -4
\end{pmatrix}
$$

Exercise:
Calculer -3C + 2D.
$$
-3C + 2D = \begin{pmatrix}
-3 + (-2) & 6 + 4 & -9 + (-4) \\
-3 + (-2) & -6 + 6 & -3 + (-6) \\
0 + (-2) & 3 + (-2) & -6 + (-8)
\end{pmatrix} = \begin{pmatrix}
-5 & 10 & -13 \\
1 & 0 & -9 \\
-2 & 1 & -14
\end{pmatrix}
$$
### Produit de deux matrices
Il faut le nombre de colonne de la 1er matrice egal au nombre de ligne de le 2eme matrice
A(n;m) X B(m;p) = C(n;p)
Example:
(2;~~3)(3~~;2)
$$
A = \begin{pmatrix}
1 & 2 & -1 \\
-1 & 3 & -1
\end{pmatrix}
$$
$$
B = \begin{pmatrix}
1 & 2 \\
-1 & 0 \\
-1 & 4
\end{pmatrix}
$$
$$
A \times B = C_{2 \times 2} \begin{pmatrix}
C_{11} & C_{12} \\
C_{21} & C_{22}
\end{pmatrix}
$$
$$
C_{11} = (1)(1) + (2)(-1) + (-1)(-1) = 1 - 2 + 1 = 0

$$
$$
C_{12} = (1)(2) + (2)(0) + (-1)(4) = 2 + 0 - 4 = -2
$$
$$
C_{21} = (-1)(1) + (3)(-1) + (-1)(-1) = -1 - 3 + 1 = -3
$$

$$
C_{22} = (-1)(2) + (3)(0) + (-1)(4) = -2 + 0 - 4 = -6

$$
$$
C = \begin{pmatrix}
0 & -2 \\
-3 & -6
\end{pmatrix}
$$
### Produit de deux matrices: A x B:
Il faut le nombre de colonne de la premier matrice egal au nombre de ligne de la 2me matrice
$$
{H}_{(n;m)} \times {B}_{(m;p)} = C_{(n;p)}
\quad \hat{D}_{\left(\frac{1}{7}2\right)} = 
$$
$$
C_{3;3}=\begin{pmatrix}
4 & 3 & 0 \\
-1 & -1 & -3 \\
3 & 0 & 1
\end{pmatrix}
$$
$$
D_{3;3}= \begin{pmatrix}
-1 & -2 \\
-1 & -3 \\
-1 & -3
\end{pmatrix}
$$
(3;~~3) x (3~~;2)
$$
C \times D = E_{3;2} = \begin{pmatrix}
e_{11} & e_{12} \\
e_{21} & e_{22} \\
e_{31} & e_{32}
\end{pmatrix}
$$
$$

e_{11} = (1)(-1) + (3)(-1) + (0)(-1) = -1 - 3 + 0 = -4
$$
$$
e_{12} = (1)(-2) + (3)(-3) + (0)(-2) = -2 - 9 + 0 = -11
$$

