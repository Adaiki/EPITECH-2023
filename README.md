# EPITECH-2023

Salut les moldus, c'est Harry, et ici c'est mon petit Github avec des tips parce que je vous aime bien

Restez pas tek1 a vie et codez bien.

## SOMMAIRE

*[BSQ ALGO](https://github.com/Adaiki/EPITECH-2023/blob/master/README.md#bsq)

## BSQ ALGO

Je vais vous faire une petite explication de l'algorithme vu en follow-up

L'algorithme consiste a utiliser des valeurs numeriques pour la map et ainsi pouvoir comparer la position actuelle avec les cases l'entourant.

Voici une map

```
.o...o
o...o.
..o...
.....o
...o..
```

Une fois transformee avec des valeurs numeriques, la map ressemblera a ceci

```
101110
011101
110111
111110
111011
```
Cette forme nous donne deja quelques informations, on peut voir sur la premiere ligne `101110` qu'il y a 4 carres de 1.

Maintenant, la partie principale de l'algo

La valeur d'une case est soit 0 (Si c'est un mur) ou la valeur de la plus petite case autour (Au dessus, a gauche et au dessus a gauche)

```
101110
011201
110111
121120
122011
```

La seule chose qui reste a faire est de trouver la plus grande valeur (sa premiere occurence).

La case trouvee est la position inferieure droite du carre, carre qui a pour taille la valeur de la case.

```
.oxx.o
o.xxo.
..o...
.....o
...o..
```
