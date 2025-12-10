# DEFI4-Arena_des_defis
📝 Description du Projet
Ce projet est une plateforme de défis de programmation amusante, conçue pour permettre aux étudiants de résoudre des problèmes interactifs, de comparer leurs solutions et d'améliorer leurs compétences en pensée computationnelle.

Le système permet de tester l'efficacité des solutions soumises, d'attribuer des scores en fonction de la difficulté du défi et de l'efficacité de la solution (nombre de tentatives, nombre d'opérations, etc.). Il maintient un classement des meilleurs programmeurs.

🎯 Objectifs
Résoudre des problèmes algorithmiques stimulants.

Comparer les performances avec d'autres solutions.

Développer une pensée computationnelle.

🧩 Défis Implémentés
Le système propose actuellement les défis suivants, chacun avec son propre score potentiel :

ID    Défi	                          Objectif	                                                        Score 
1     Le Compte est Bon	        Trouver une combinaison d'opérations pour atteindre un nombre cible.	    20
2	    Mastermind Algorithmique	Deviner une séquence secrète de nombres en minimum d'essais.	            35
3	    Course de Robots	        Trouver le chemin le plus court dans un labyrinthe.	                      10
4	    Tri Ultime	              Trier un tableau avec des contraintes spécifiques.	                      25



🛠️ Installation et Compilation
Ce projet est écrit en langage C. Pour compiler et exécuter le programme, vous devez disposer d'un compilateur C (comme GCC ou Clang).

1. Cloner le dépôt
Bash

git clone https://github.com/Khalil-atallah/DEFI4-Arena_des_defis
cd DEFI4-Arena_des_defis
2. Compilation (Lien corrigé)
La compilation doit inclure tous les fichiers sources .c du projet. Attention : Pour éviter l'erreur de liaison undefined reference to 'ajouter_submission', assurez-vous d'inclure addsubmission.c.

Bash

gcc -o my_program main.c ui.c defi3.c addsubmission.c date_submission.c ecriredansclassement.c ajouterligne.c affichestanding.c affichestats.c .\defi4.c defi1.c defi2.c .\statspersonnel.c .\affichehistorique.c

3. Exécution du Programme
Après la compilation, exécutez le programme :

Bash

./my_program



⚙️ Structure des Fichiers
  Fichier                          	Description
  
main.c	                  Point d'entrée du programme .
ui.c	                    Gère l'interface utilisateur, la navigation dans les menus et les appels aux fonctions de défi.
ajouterligne.c	          Ajoute le score d'un joueur au classement (avant le tri).
ecriredansclassement.c	  Contient la fonction mise_a_jour qui lit, trie (via qsort), et réécrit le classement (standing2.txt).
affichestanding.c	        Affiche le contenu du classement standing2.txt.
addsubmission.c	          Enregistre les statistiques de soumission pour chaque défi (temps, nombre d'essais).
affichehistorique.c       Affiche l'historique de touts les soumissions effectuées.
affichestats.c            Affiche les statistiques de touts les defis .
statspersonnel.c          Ajouter à l'historique la soumission effectuée .
defi1.c                   Implémentation du défi "Le Compte est Bon" .
defi2.c                   Implémentation du défi "Mastermind Algorithmique" .
defi3.c	                  Implémentation du défi "Course de Robots" .
defi4.c                   Implémentation du défi "Tri Ultime" .
date_submission.c	        Fournit la fonction timing() pour horodater les soumissions.
standing2.txt	            Fichier de données contenant le classement des joueurs.





👤 Auteur
Khalil Atallah
