# JEE-Activite-6

Le but de cette activite est de reprendre l'exemple de la démo pour maitriser les concepts fondamentaux de Angular.

### Travail à faire ###

1. Créer un projet Angular avec la commande `ng new my-angular-project`.
2. Créer une barre de navigation sur le composant App.
3. Créer le modele 'Product' avec les champs suivants:
     - id de type number,
     - name de type String,
     - price de type number,
     - checked de type boolean.
4. Définir le fichier 'data/db.json' pour le stockage des données.
5. Créer les composants suivants : 
     - Home => `ng g c home`,
     - new-product => `ng g c new-product`,
     - products => `ng g c products`.
6. Créer le service 'services/product' => `ng g s services/product`.
7. Définir quelques opérations de gestion des produits :
    - Consulter tous les produits avec pagination,
    - Chercher des produits avec un mot clé,
    - Ajouter un produit,
    - Supprimer un produit,
    - La possibilité de changer la valeur booleanne de l'attribut 'checked' avec un bouton.

=> Vidéo à utiliser comme ressource principale : https://www.youtube.com/watch?v=1uTIemRcZWM&authuser=0

### Présentation d'Angular ### 

![angular-3-logo](https://github.com/Ikramouslih/JEE-Activite-6/assets/60039200/ebef6263-bf31-4059-96b0-1e8b83434e09)

Angular est un framework JavaScript open-source basé sur TypeScript. Il permet de construire des applications web dynamiques, single-page (SPA) et multiplateformes. Il offre un ensemble complet d'outils et de fonctionnalités pour simplifier le processus de développement et améliorer l'expérience utilisateur.

Principales caractéristiques et avantages d'Angular :
- Structure MVC : Facilite la séparation des responsabilités et la maintenance du code. Cela rend le développement plus structuré et évolutif.
- Deux-way data binding : Toute modification effectuée dans l'interface utilisateur est automatiquement reflétée dans les données sous-jacentes, et vice versa. Cela permet une synchronisation fluide entre les vues et les modèles de données.
- Injection de dépendances : Facilite la gestion des dépendances entre les composants. Cela rend le code plus modulaire, réutilisable et testable.
- Routing : Permet la navigation entre différentes vues et la gestion des URL. Cela permet la création d'applications à pages multiples tout en maintenant une expérience utilisateur fluide.
- Validation des formulaires : Simplifient la validation des données côté client. Il fournit également des mécanismes pour personnaliser les règles de validation selon les besoins de l'application.
- Performances optimisées : Utilise des techniques telles que le lazy loading, la détection du changement, et la compilation juste-à-temps (JIT) ou à l'avance (AOT).
- Large communauté et écosystème : Des nombreuses ressources, bibliothèques et extensions disponibles pour faciliter le développement.

### La configuration et les dependences du projet ### 

Ce projet a été généré avec [Angular CLI](https://github.com/angular/angular-cli) version 16.0.1.

- Bootstrap & Bootstrap-icons : 
Une bibliothèque open-source de développement front-end pour la conception de sites et d'applications web. Elle fournit des styles CSS prédéfinis, des composants JavaScript et des icônes pour faciliter la création d'interfaces utilisateur esthétiques et responsives.
    * Installation : `npm i bootstrap bootstrap-icon`
- Json-server : 
JSON Server est un outil simple et léger permettant de créer rapidement une fausse API RESTful en utilisant un fichier JSON comme source de données. Il fournit un serveur web minimaliste qui expose les données JSON comme des endpoints REST.
    * Installation : `npm install -g json-server`
    * Lancement du json-server sur le port 8089 : `json-server -w data/db.json -p 8089`

### L'interface de l'Output et les fonctionnalités implémentées ### 

- La liste des produits et la pagination: 

<img width="960" alt="Screenshot (14)" src="https://github.com/Ikramouslih/JEE-Activite-6/assets/60039200/83552ed4-f41c-4b26-ac34-a44d69dd4123">

- La possibilité de changer la valeur booléeanne de l'attribut 'checked' avec un bouton.

<img width="960" alt="Screenshot (3)" src="https://github.com/Ikramouslih/JEE-Activite-6/assets/60039200/5b2e8a0e-b4a0-4628-acb3-8f00cd6fcd58">

<img width="960" alt="Screenshot (4)" src="https://github.com/Ikramouslih/JEE-Activite-6/assets/60039200/203a3f9d-b2ce-474f-a76c-a9b4e1d76467">

- La recherche d'un produit selon un mot clé : 

<img width="960" alt="Screenshot (13)" src="https://github.com/Ikramouslih/JEE-Activite-6/assets/60039200/5429d389-8bc8-4863-91e1-e7e49d6a5706">

- Le formulaire d'ajout d'un produit :

<img width="960" alt="Screenshot (10)" src="https://github.com/Ikramouslih/JEE-Activite-6/assets/60039200/3eb322ef-15e5-4637-9e30-81a35674a817">

<img width="960" alt="Screenshot (11)" src="https://github.com/Ikramouslih/JEE-Activite-6/assets/60039200/801da4a0-fe46-4394-8064-b233c6b99416">

<img width="960" alt="Screenshot (12)" src="https://github.com/Ikramouslih/JEE-Activite-6/assets/60039200/4bc34a1b-c729-4529-8e62-596a5afcf682">

- La suppression d'un produit : 

<img width="960" alt="Screenshot (8)" src="https://github.com/Ikramouslih/JEE-Activite-6/assets/60039200/da761da7-d455-46eb-8a5b-2ef54131306b">

<img width="960" alt="Screenshot (9)" src="https://github.com/Ikramouslih/JEE-Activite-6/assets/60039200/00b4dc7b-f809-408a-8bff-ab1442fb7ce0">

## Development server
Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding
Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build
Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests
Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests
Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help
To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
