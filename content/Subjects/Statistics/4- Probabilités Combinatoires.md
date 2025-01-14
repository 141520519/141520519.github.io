---
title: 4- Probabilités Combinatoires
tags:
  - statistics
  - lecture
  - exercise
  - latex
draft: false
subject: Statistics
professor: Amina Dankar
last_modified: 2025-1-14
---
# **Conclusion**

- On tire _p_ éléments de _n_ :
  - **Avec ordre** :
    - Avec répétition : Arrangement avec répétition : _n<sup>p</sup>_
    - Sans répétition : Arrangement sans répétition :  
      A<sup>p</sup><sub>n</sub> = $$ \frac{m!}{(m-p)!} $$  
      - Si _p_ = _m_ alors :  
        A<sup>m</sup><sub>m</sub> = $$ \frac{m!}{(m-m)!} $$ = $$ \frac{m!}{0!} $$ = $$ \frac{m!}{1} $$ = _m!_ (permutation)
  - **Sans ordre** :
    - Sans répétition : Combinaison :  
      C<sup>p</sup><sub>m</sub> = $$ \frac{m!}{p!(m-p)!} $$

---

# **Propriétés**

- A<sup>m</sup><sub>m</sub> = _m_ ex : A<sup>5</sup><sub>5</sub> = 5 / A<sup>5</sup><sub>8</sub>  
- A<sup>m</sup><sub>m</sub> = _m!_
- C<sup>m</sup><sub>m</sub> = _m_
- C<sup>1</sup><sub>m</sub> = 1

---

# **Remarques**

- **Successive** : Avec ordre
- **Avec remise** : Avec répétition
- **Simultanément / Au hasard** : Sans ordre
- **U** : ou : +
- **∩** : et : ×

---

# **Exemple**

On considère un jeu de 32 cartes dans lequel on a 4 couleurs : trèfle, pique, carreau et cœur. Dans chaque couleur, on trouve 8 valeurs : as, roi, dame, valet, dix, neuf, huit, sept.

On tire au hasard 5 cartes.

## **a) Combien de tirages différents peut-on obtenir ?**

C<sup>5</sup><sub>32</sub> = $$ \frac{32!}{5!(32-5)!} $$ = $$ \frac{32!}{5!27!} $$  

C<sup>5</sup><sub>32</sub> =  
$$
\frac{32 \times 31 \times 30 \times 29 \times 28}{1 \times 2 \times 3 \times 4 \times 5}
$$  
= 201 376 tirages différents.

---

## **b) Combien de tirages différents peut-on obtenir contenant :**

### **1) 5 Cœurs ou 5 Carreaux**

C<sup>5</sup><sub>8</sub> + C<sup>5</sup><sub>8</sub> = $$ \frac{8!}{5!(8-5)!} $$ + $$ \frac{8!}{5!(8-5)!} $$  

= $$ \frac{6 \times 7 \times 8}{1 \times 2 \times 3} $$ + $$ \frac{6 \times 7 \times 8}{1 \times 2 \times 3} $$  

= 56 + 56 = **112**

---

### **2) 2 Cœurs et 3 Carreaux**

C<sup>2</sup><sub>8</sub> × C<sup>3</sup><sub>8</sub> = $$ \frac{8!}{2!(8-2)!} $$ × $$ \frac{8!}{3!(8-3)!} $$  

= $$ \frac{7 \times 8}{1 \times 2} $$ × $$ \frac{6 \times 7 \times 8}{1 \times 2 \times 3} $$  

= $$ \frac{56}{2} $$ × $$ \frac{336}{6} $$  

= 28 × 56 = **1 568**

---

### **3) Aucun As**

32 - 4 = 28 cartes sans As.  
C<sup>5</sup><sub>28</sub> = $$ \frac{28!}{5!(28-5)!} $$  

= $$ \frac{28 \times 27 \times 26 \times 25 \times 24}{1 \times 2 \times 3 \times 4 \times 5} $$  

= **98 270**

---

### **4) Les 4 As et 1 autre**

C<sup>4</sup><sub>4</sub> × C<sup>1</sup><sub>28</sub> = 1 × 28 = **28**

---

### **5) Au moins un As**

(C<sup>1</sup><sub>4</sub> × C<sup>4</sup><sub>28</sub> + C<sup>2</sup><sub>4</sub> × C<sup>3</sup><sub>28</sub> + C<sup>3</sup><sub>4</sub> × C<sup>2</sup><sub>28</sub> + C<sup>4</sup><sub>4</sub> × C<sup>1</sup><sub>28</sub>)  

Nombre total de tirages - Nombre de tirages sans aucun As :  
201 376 - 98 270 = **103 096**