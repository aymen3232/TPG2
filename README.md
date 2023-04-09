# TPGit2


Fin du TP2

EXécution de la commande git reflog pour git reset --hard branch2

TP2 :

Étape 1:

Créer un nouveau dossier pour le projet et initialiser un dépôt Git local: mkdir nom_du_dossier && cd nom_du_dossier && git init
Créer un fichier README.md et ajouter une brève description du projet: touch README.md puis ouvrir le fichier avec un éditeur de texte pour y ajouter une description.
Faire un commit pour enregistrer le fichier ajouté: git add README.md && git commit -m "Ajout du fichier README.md"

Étape 2:

Apporter des modifications au fichier README.md sans les commiter: modifier le contenu du fichier README.md.
Utiliser git stash pour sauvegarder temporairement vos modifications: git stash
Revenir aux modifications sauvegardées en utilisant git stash apply ou git stash pop: git stash apply

Étape 3:

Chaque membre crée une nouvelle branche pour travailler sur une fonctionnalité distincte: git branch nom_de_la_branche
Faire des commits sur chaque branche: git checkout nom_de_la_branche && git add fichier_modifié && git commit -m "Description du commit"
Utiliser git rebase pour réorganiser et "nettoyer" l'historique des commits avant de fusionner les branches: git checkout branche_principale && git rebase nom_de_la_branche

Étape 4:

Chaque membre crée une nouvelle branche pour travailler sur une autre fonctionnalité: git branch nom_de_la_branche
Faire plusieurs commits sur chaque branche: git checkout nom_de_la_branche && git add fichier_modifié && git commit -m "Description du commit"
Utiliser git cherry-pick pour sélectionner et appliquer un commit spécifique d'une branche sur une autre: git checkout branche_principale && git cherry-pick id_du_commit

Étape 5:

Introduire volontairement un bogue dans le projet et commiter les modifications: modifier le code pour ajouter le bogue && git add fichier_modifié && git commit -m "Ajout du bogue"
Utiliser git bisect pour identifier le commit qui a introduit le bogue: git bisect start && git bisect bad HEAD && git bisect good id_du_commit_sans_bug
Réparer le bogue et commiter les modifications: modifier le code pour corriger le bogue && git add fichier_modifié && git commit -m "Correction du bogue"

Étape 6:

Créer plusieurs tags pour marquer différentes versions du projet: git tag nom_du_tag
Utiliser git tag pour afficher les tags existants: git tag
Utiliser git checkout pour basculer entre différentes versions du projet en utilisant les tags: git checkout nom_du_tag

Étape 7:

Apporter plusieurs modifications au projet et effectuer des actions Git, telles que des commits, des fusions et des rebases.
Utiliser git reflog pour afficher l'historique des actions Git: git reflog
Utiliser git reflog pour récupérer un commit perdu ou revenir à un état antérieur du projet: git reset --hard id_du_commit

