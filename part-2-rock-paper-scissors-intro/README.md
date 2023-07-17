🧱📃✂️ **Le cycle TDD : Intro du Kata Rock Paper Scissors**

Nous arrivons à notre premier exercice dans ce cours, où nous allons commencer à appliquer ce que nous avons appris. 💪

Dans cette partie, je vais vous présenter l'exercice que nous voulons aborder, puis nous allons couvrir un peu de théorie dont vous aurez besoin pour le faire en utilisant le **TDD**. Ensuite, je vous ferai démarrer en faisant les premiers tests avec vous avant que vous ne continuiez et que vous ne terminiez le **Kata**.

Mais plantons le décor de ce que nous essayons de faire ici. 🌱

Ce **kata** est très simple. Il s'agit de mettre en œuvre le jeu de _pierre-papier-ciseaux_. 🧱📃✂️

Il s'agit d'un jeu à deux joueurs, si vous ne le connaissez pas, où chaque joueur choisit secrètement une pierre, un papier ou des ciseaux dans son dos. C'est un geste de la main qu'ils tiennent, puis les deux joueurs révèlent leur choix en même temps avec un geste de la main. 🤚✋

![Rock Paper Scissors](https://en.wikipedia.org/wiki/Rock_paper_scissors#/media/File:Rock-paper-scissors.svg "Rock Paper Scissors")

En règle générale, on compte jusqu'à trois et, à trois, les deux joueurs révèlent leur choix en même temps. L'exercice consiste à créer un backend, une fonction _TypeScript_ pour le jeu qui détermine qui gagne entre les deux joueurs. Il s'agit donc de dire, le joueur 1 a choisi les ciseaux, le joueur 2 a choisi le papier, qui gagne ? Elle accepte les mouvements des joueurs en entrée, les traite selon les règles et renvoie le résultat : quelqu'un a gagné ou il y a eu égalité. 🏆

Ce que nous ferons également dans ces deux premiers exercices, c'est que je vous fournirai les cas de test. Voici les cas de test, et il s'agit d'une liste exhaustive des mouvements possibles :

📝 **Cas de test** :

|  Player Move  |  Opponent Move  |  Result  |
|:-------------:|:---------------:|:--------:|
| Paper | Rock | Player Wins | 
| Paper | Scissors | Player Loses | 
| Paper | Paper | Tie | 
| Rock | Scissors | Player Wins | 
| Rock | Paper | Player Loses | 
| Rock | Rock | Tie | 
| Scissors | Paper | Player Wins | 
| Scissors | Rock | Player Loses | 
| Scissors | Scissors | Tie | 

Vous n'êtes pas obligé de les utiliser, ils sont juste là pour vous aider avec les tests qui doivent être écrits pendant que vous vous habituez encore à la sensation de **TDD**. Je vous donne donc les cas de test, vous n'avez pas à les découvrir par vous-même. L'objectif ici est de se concentrer sur l'application des bases du **TDD**, étant donné un problème très simple et les cas de test à utiliser, nous commençons par un exercice intentionnellement simple. 😉🧪

Il n'y a pas de pièges cachés. Il n'y a pas d'algorithme secret ou de secret spécial, comme une implémentation vraiment intelligente que nous recherchons. Il s'agit littéralement d'un problème qui peut être résolu avec quelques instructions. Nous faisons cela parce qu'au début, je veux que vous vous concentriez sur ce que cela fait de faire du **TDD** sans les autres distractions telles que la réflexion sur les algorithmes.

Très bien, maintenant que nous avons couvert l'exercice lui-même, nous allons aborder la théorie que nous devons appliquer en faisant l'exercice.

Dans la prochaine partie, nous aborderons **les 3 lois du TDD**. 📚🧪