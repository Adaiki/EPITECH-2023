# Sokoban

# Sommaire
* ## [Le jeu](https://github.com/Adaiki/EPITECH-2023/blob/master/sokoban.md#le-jeu-1)
* ## [Map](https://github.com/Adaiki/EPITECH-2023/blob/master/sokoban.md#map-1)
* ## [Déplacements et collisions](https://github.com/Adaiki/EPITECH-2023/blob/master/sokoban.md#déplacements-et-collisions-1)
* ## [État de la partie](https://github.com/Adaiki/EPITECH-2023/blob/master/sokoban.md#état-de-la-partie-1)
* ## [Fonction du jeu](https://github.com/Adaiki/EPITECH-2023/blob/master/sokoban.md#fonction-du-jeu-1)

## Le jeu

Dans sokoban, le joueur doit ranger des caisses sur des cases cibles. Il peut se déplacer dans les quatre directions, et pousser (mais pas tirer) une seule caisse à la fois. Une fois toutes les caisses rangée, le niveau est réussi.


## Map

**Récupération de la map**

Les fonctions autorisées utiles pour récupérer la map sont

* (f)open
* (f)close
* (f)read
* getline

Vous pouvez utiliser `(f)open, (f)read et (f)close` ou découvrir une fonction qui est `getline`, à vous de choisir

(Vous devriez conserver une copie intacte de la map, petit conseil)

**Vérification de la map**

Une map valide a 

* ~~Des **murs (#) fermés**~~ Les murs ne doivent pas forcement etre fermes, mais faites attention a ne pas segfault en en sortant
* **Un seul** player (P)
* Autant (ou plus) de boites (X) que de rangements (O)
* Est seulement composée de "#OXP \n"

## Déplacements et collisions

* Pour déplacer le personnage (P), et que c'est un espace qui le suit, inversez les deux caractères (`P ` deviendra ` P`)
* Si c'est un X qui est après, faites de même avec le X (`PX ` deviendra `P X` puis ` PX`)
* Si le personnage est suivi d'un X et d'un O, déplacez le X sur le O (`PXO` deviendra ` PX`)
	* Si vous marcher juste sur un O, afficher P à sa place (`PO` deviendra ` P`)
	* Si vous enlevez un P ou un X d'un O, réaffichez le (`PX ` deviendra ` PX `, et en bougeant encore ` OPX`)
* Sinon, ne bougez rien
	
Pour récupérer la direction, vous devez récupérez l'input (les flèches du claviers), renseignez vous sur les fonctions `getch` et `keypad`
	
Vous pouvez gerer differement les deplacements (CF http://www.cs.ukzn.ac.za/~hughm/os/notes/ncurses.html)

## État de la partie

Si tous les X sont sur des O, la partie est gagnée.
Si un X est impossible à bouger (càd dans un coin), la partie est perdue.

```
##
#X
```

## Fonction du jeu

La touche espace sert a réinitialiser la map (souvenez vous de la copie de la map dont j'ai parlé au début)
