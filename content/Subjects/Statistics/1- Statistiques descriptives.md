---
title: 1- Statistiques descriptives
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
| Class       | Effectifs (ni) | Fréquence (fi)        | Pourcentage (pi)              | Fréquence cumulative croissante | Fréquence cumulative décroissante |
| ----------- | -------------- | --------------------- | ----------------------------- | ------------------------------- | --------------------------------- |
| [30 - 40 [  | 11 (n1)        | 11/N = 11/200 = 0.055 | fi x 100 = 100 x 0.055 = 5.5% | 11                              | N = 200                           |
| [40 - 50 [  | 26 (n2)        | 0.13                  | 13%                           | ni + ni+1 = 11 + 26 = 37        | N - ni+1 = 200 - 11 = 189         |
| [50 - 60 [  | 63 (n3)        | 0.315                 | 31.5%                         | 100                             | 163                               |
| [60 - 70 [  | 31 (n4)        | 0.155                 | 15.5%                         | 131                             | 100                               |
| [70 - 80 [  | 29 (n5)        | 0.145                 | 14.5%                         | 160                             | 69                                |
| [80 - 90 [  | 21 (n6)        | 0.105                 | 10.5%                         | 181                             | 40                                |
| [90 - 100 [ | 19 (n7)        | 0.095                 | 9.5%                          | 200                             | 19                                |
| Total       | 200            | 1                     | 100%                          |                                 |                                   |

**Notes:**

$$
N = \sum n_i
\quad \text{et} \quad 
\sum f_i = 1 \quad \left( \frac{\sum n_i}{N} = \frac{N}{N} = 1 \right)
$$

### Classe amplitude:
- Amplitude de classe [ a - b [: \(a_i = b - a\)
    - Exemple: [45 - 60 [: \(a_i = 60 - 45 = 15\)
- L'amplitude de chaque classe est 10.

### Centre de classe [a - b[ :
$$
X_i = \frac{a + b}{2}
$$

### Moyenne:
$$
\bar{X} = \frac{\sum (n_i \times X_i)}{N}
$$

**Exemple**:
$$
\frac{12800}{200} = 64
$$

### Histogramme:
![[Statistics-IMG-0007.png]]

### Variance:
$$
V(x) = \frac{\sum n_i \times x_i^2}{N} - \bar{x}^2
$$

$$
\bar{x} = \frac{\sum n_i \times x_i}{N} = \frac{12800}{200} = 64
$$

$$
V(x) = \frac{874000}{200} - 64^2 = 274 \quad (\text{sans unité})
$$

### Ecart type:
$$
\sigma(x) = \sqrt{V(x)} = \sqrt{274} = 16.55
$$

### Médiane par calcul et graphiquement:
- Fonction de réparation:
![[Statistics-IMG-0008.jpg]]

#### Par calcul:
$$
\frac{N}{2} = 100 \quad \Rightarrow \quad M_e \in [50 - 60[
$$

$$
M_e = l_i + a_i \left( \frac{\left( \frac{N}{2} \right) - n_{i-1} c_c}{n_i} \right)
$$

$$
M_e = 50 + 10 \left( \frac{100 - 37}{63} \right)
= 50 + 10 \times 1 = 60
$$
