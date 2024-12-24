---
title: 2- Statistiques descriptives
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
## 1) Déterminer le tableau des fréquences

| Classe      | Fréquence | fi          | pi    | ni.cc | ni.cd  | xi  | ni x xi |
| ----------- | --------- | ----------- | ----- | ----- | ------ | --- | ------- |
| [ 0 - 4 [   | 13        | 13/130 = 0.1 | 10%   | 13    | N = 130 | 2   | 26      |
| [ 4 - 8 [   | 26        | 0.2         | 20%   | 39    | 117    | 6   | 156     |
| [ 8 - 12 [  | 39        | 0.3         | 30%   | 78    | 91     | 17  | 390     |
| [ 12 - 16 [ | 22        | 0.17        | 17%   | 100   | 52     | 14  | 308     |
| [ 16 - 20 [ | 19        | 0.148       | 14.6% | 119   | 30     | 18  | 342     |
| [ 20 - 24 [ | 11        | 0.084       | 8.4%  | 130   | 11     | 22  | 242     |
| **Total**   | 130       | 130/130 = 1  | 100%  |       |        |     | 1464    |

## 2) Déterminer le tableau de pourcentages

| Classe      | pi (%) |
| ----------- | ------ |
| [ 0 - 4 [   | 10%    |
| [ 4 - 8 [   | 20%    |
| [ 8 - 12 [  | 30%    |
| [ 12 - 16 [ | 17%    |
| [ 16 - 20 [ | 14.6%  |
| [ 20 - 24 [ | 8.4%   |

## 3) Lever les effectifs cumulés Croissants (ni.cc)

| Classe      | ni.cc |
| ----------- | ----- |
| [ 0 - 4 [   | 13    |
| [ 4 - 8 [   | 39    |
| [ 8 - 12 [  | 78    |
| [ 12 - 16 [ | 100   |
| [ 16 - 20 [ | 119   |
| [ 20 - 24 [ | 130   |

## 4) Trouver les effectifs Cumulés Décroissants (ni.cd)

| Classe      | ni.cd |
| ----------- | ----- |
| [ 0 - 4 [   | 130   |
| [ 4 - 8 [   | 117   |
| [ 8 - 12 [  | 91    |
| [ 12 - 16 [ | 52    |
| [ 16 - 20 [ | 30    |
| [ 20 - 24 [ | 11    |

## 5) Tracer l'histogramme des ni.C.C.
![[Statistics-IMG-0009.png]]

## 6) Déterminer la moyenne

La formule de la moyenne est :
$$
\bar{X} = \frac{\sum n_i \times x_i}{N} = \frac{1464}{130} = 11,25
$$

## 7) Trouver le mode par calcul et graphiquement

### Mode graphiquement :
Histogramme des effectifs:
![[Statistics-IMG-0010.jpg]]

### Mode par calcul :
Le plus grand effectif est 39, donc le mode se trouve dans l'intervalle [8 - 12[ :
$$
M_o = l_i + a_i \left( \frac{n_i - n_{i-1}}{n_i - n_{i-1} + n_i - n_{i+1}} \right)
$$
$$
M_o = 8 + 4 \left( \frac{39 - 26}{39 - 26 + 39 - 22} \right)
= 8 + 4 \times \frac{13}{30} = 9.73
$$

## 8) Trouver la médiane par calcul et graphiquement

### Médiane graphiquement :
Fonction de réparation :
![[Statistics-IMG-0011.jpg]]

### Médiane par calcul :
$$
\frac{N}{2} = \frac{130}{2} = 65 \quad \Rightarrow \quad M_e \in [8 - 12[
$$
$$
M_e = l_i + a_i \left( \frac{\left( \frac{N}{2} \right) - n_{i-1} c_c}{n_i} \right)
$$
$$
M_e = 8 + 4 \left( \frac{65 - 39}{39} \right) = 8 + 4 \times 0.66 = 10.66 \quad (\text{unité})
$$
