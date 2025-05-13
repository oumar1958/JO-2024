# Analyse d’une base de données sur les médailles aux Jeux Olympiques de 2024
## Objectif du projet
L’objectif de ce projet est de rendre les analyses de bases de données accessibles à tous ceux qui souhaitent extraire des informations sur les Jeux Olympiques de 2024. Notre objectif est de simplifier l’interprétation des résultats afin qu’ils soient compréhensibles par tous, quel que soit leur niveau de data science.
## Jeu de données
## Source des données
L’ensemble de données que nous avons utilisé dans ce projet est extrait de ce lien : 
https://www.data.gouv.fr/fr/datasets/paris-2024-resultats-des-medailles-pour-chaque-discipline-olympique/
Il répertorie toutes les médailles remportées lors des Jeux Olympiques.
## Description
L’ensemble de données contient 11 variables et 1045 observations.
Medal_type : Or / Argent / Bronze
Medal_code : respectivement 1 / 2 / 3
Medal_date : Date de l’événement
Nom : Prénom et NOM DE L’ATHLÈTE
Sexe : M pour les hommes et W pour les femmes
Discipline : Épreuve dans laquelle l’athlète a remporté sa médaille
Code_Discipline : 3 lettres
Épreuve : catégorie dans laquelle l’athlète a remporté sa médaille
url_event : URL de l’événement
Pays : Pays représenté par l’athlète
Country_code : 3 lettres représentant le pays

Toutes les catégories et valeurs sont en français dans cette base de données.

## Structure du référentiel
Le référentiel est organisé de la manière suivante :

• data : contient le jeu de données

• scripts : répertoire des fonctions :


analyse_data, fonctions d’analyse 

• : fonctions du nœud Athlète 

• : fonctions du nœud Pays 

• : fonctions du nœud Statistiques générales

• : réalise plusieurs podiumsathlete.pycountry.pygeneral_statistics.pypodium.py


interface, fonctions de l’interface : 

• : fonction principale 

• : crée des menus 

• : message de bienvenueapp.pymenu.pywelcome.py


manipulation_data, manipulation fonctions : 

• : fichier avec toutes les constantes utilisées 

• : compte les lignes d’un sous-ensemble 

• : charge et nettoie la base de données 

• : recherche dans la base de donnéesconstants.pycount.pyload.pysearch.py


main.py, le script principal


• Tests : répertoire des tests de fonction :

test_analyse_data :
• 
• 
• 
• test_athlete.pytest_country.pytest_general_statistics.pytest_podium.py


test_interface :
• test_menu.py


test_manipulation_data :
• 
• test_count.pytest_search.py


• .gitignore

• requirements.txt


# Configuration et utilisation
Avant d’utiliser notre programme, assurez-vous d’avoir la configuration suivante :

## Configuration et utilisation
Installation
Clonez le dépôt Git sur votre machine locale :
https://gitlab-mi.univ-reims.fr/arvo0004/managlent-proj-digit.git
Accédez au répertoire cloné dans votre terminal :
cd managlent-proj-digit
Installer ou mettre à niveau pip :
python -m pip install --upgrade pip
Installez les dépendances requises à l’aide de pip :
pip install -r requirements.txt


## Usage
Exécutez cette ligne de code pour lancer l’application :
python ./scripts/main.py

## Opération
Notre algorithme est organisé comme un arbre de décision. À chaque étape, l’utilisateur doit choisir parmi plusieurs options pour déterminer l’analyse parfaite qu’il souhaite.
Ils peuvent quitter le programme à tout moment et faire autant d’analyses qu’ils le souhaitent.
## Auteur
ALLAWAN Oumar Abdramane
