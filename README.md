![Learn@Home](https://raw.githubusercontent.com/waleedos/2023_P3__Learn-Home/main/icons/1599557620417_Learn%40Home.png)

# Designez une application Python adaptée aux besoins d'un client

## Préambule
Projet N°3 réalisé dans le cadre de la formation Développeur d'Applications Python d'OpenClassrooms.
Ce programme permet de à la fin d'avoir les Compétences suivantes:

## Compétences évaluées
* Prototyper une solution technique pour un client avec les modèles de domaine et maquettes
* Gérer un projet avec les méthodologies agiles
* Définir les exigences fonctionnelles de l’application à partir du besoin client


## Scénario
Vous êtes employé depuis 5 ans chez Dev4U, une entreprise de services du numérique de 120 collaborateurs comportant deux entités de développement logiciel  : 

une entité spécialisée dans le développement d’applications mobiles, qui comprend 10 personnes  ;
une dédiée au web, qui comprend 8 personnes.

![Dev4U](https://raw.githubusercontent.com/waleedos/2023_P3__Learn-Home/main/icons/Capture%20d%E2%80%99%C3%A9cran_2023-04-26_16-46-21.png)

Vous êtes le lead développeur de l’entité Web.

Vous recevez un message de votre manager avec une bonne nouvelle…
```
Thomas : Hello ! Ça va ? Je sors d’une réunion avec Learn@Home ! Et j’ai un projet pour toi  ! 

Vous : Ça va et toi ? Super ! C’est quoi ce projet ? 😃

Thomas : Learn@Home est une association qui met en relation des enfants en difficulté scolaire avec des tuteurs bénévoles. En gros, leur objectif est de permettre à tout élève, où qu’il soit, d’avoir accès à un soutien scolaire à distance. Ils nous ont confirmé qu’ils voulaient travailler avec nous sur leur projet de site web. 💪🚀

Vous : Génial ! À quoi servira leur site ? 

Thomas : Ils veulent permettre à leurs élèves et à leurs bénévoles de communiquer plus facilement, directement depuis leur site. Jusqu’alors ils utilisaient surtout WhatsApp et les SMS !

Vous : Ah oui c’est un beau challenge !

Thomas : Je voulais te proposer de gérer ce projet  : ton rôle serait de cadrer ce projet puis de coordonner tous les développements avec l’équipe. C’est un projet ambitieux et intéressant !

Vous : Merci ! 😃 Très beau projet en effet, j’ai hâte de démarrer. Tu m’envoies plus d’éléments ?

Thomas : Oui bien sûr, je t’envoie un mail dès demain.
```

## Les Balises et informations visées par ce Scarpp

Name | Description
------------|------------
product_page_url | Le lien (URL) de la page du livre
universal_ product_code (upc) | Le code unique (upc) de chaque livre 
title | Le titre du livre
price_including_tax | Le prix du livre (TTC)
price_excluding_tax | Le prix du livre (HT)
number_available | Quantité disponible en stock
product_description | La description du livre
category | La catégorie du Livre
review_rating | La note du livre
image_url | Le lien (URL) de l'image du livre





## Prerequisites
* python 3
* Requests
* CSV
* BeautifulSoup 4
* os


## Instructions générales

### Clonage ou téléchargement
Clonez cette repositoire    : https://github.com/waleedos/2023_P2__book-scraper
Ou bien 
Télécharger le zip          : https://github.com/waleedos/2023_P2__book-scraper/archive/refs/heads/main.zip

### Création d'un nouvel environnement virtuel :
Une fois dézippé, et quand vous etes dans votre environnement, mettez vous dans ce dossier sur la racine

Ouvrez un terminal et créez votre environnement virtuel à l'aide de la commande suivante : 
```
python -m venv env
```
### Activation de votre nouvel environnement virtuel :
Activer votre nouvel environnement virtuel à l'aide de la commande suivante :
```
source env/bin/activate
```
### Mise à jour de votre environnement :
Remplire et installer les modules prerequis à partir de du fichier "requirements.txt" par la commande suivante:
```
pip install -r requirements.txt
```
## Fonctionnement :
Mettez vous a la racine du repertoire "le-scrypt" avec la commande suivante :
```
cd le-scrypt
```

Démarrez le scrypt avec la commande :
```
python main.py
```
Ou bien
```
python3 main.py
```
## Mes suggestions pour l’amélioration de ce Script : 
Utiliser une bibliothèque de scraping dédiée, telle que Scrapy, pour faciliter grandement  la collecte des données, car elle est conçue spécifiquement pour cette tâche et offre des fonctionnalitées avancées telles que la gestion des proxies, le traitement en parallèle des pages, la gestion de la pagination, etc. 

Mettre tout le catalogue du site internet dans un seul fichier .CSV tout en ajoutant une colonne pour connaître les catégories, cela rendra la lecture et l’analyse des données beaucoup plus facile.

Ajouter des fonctions de validation  telles que la vérification de la structure des données, la validation des champs, etc, pour s'assurer que les données collectées sont correctes et éviter les erreurs : Il est important de valider les données collectées pour éviter les erreurs dans le traitement des données.

Ajouter une gestion d'erreurs plus robuste pour éviter les plantages du programme en cas d'erreur : Le scraping peut être assez imprévisible, donc il est important d'avoir une gestion d'erreurs solide pour éviter que le programme plante en cas d'erreur. Les erreurs courantes peuvent inclure une connexion interrompue, un serveur indisponible, une page indisponible, etc.

Utiliser des fonctions de log qui permettent de suivre les activités du programme, telles que les requêtes HTTP, les réponses, les erreurs, etc,  pour faciliter le débogage : Cela peut aider à identifier les problèmes plus rapidement.

Éviter les boucles imbriquées pour améliorer la lisibilité et les performances du code : Les boucles imbriquées peuvent rendre le code difficile à lire et à maintenir, en particulier pour les projets plus importants. Il est important de limiter l'utilisation de boucles imbriquées pour améliorer la lisibilité et les performances du code.

Utiliser des outils d'analyse de code tels que pylint pour détecter les erreurs et les problèmes de style : Les outils d'analyse de code peuvent aider à détecter les erreurs et les problèmes de style dans le code. Pylint est un outil populaire pour Python qui peut détecter les erreurs de syntaxe, les erreurs de style, les erreurs de logique, etc.

Optimiser le code pour améliorer les performances, par exemple en utilisant des techniques de traitement par lots pour éviter de surcharger les serveurs cibles : Le scraping peut être une tâche gourmande en ressources, donc il est important d'optimiser le code pour améliorer les performances et éviter de surcharger les serveurs cibles. Les techniques de traitement par lots peuvent aider à réduire la charge sur les serveurs en collectant les données en blocs plutôt que page par page.

### Powered by EL-WALID EL-KHABOU
