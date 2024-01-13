Commande :

Etape 1

- rails new Le_Carnet_des_Voyages -c tailwind -d postgresql
- rails g model User nom:string email:string
- rails g model Trip destination:string description:text date_debut:date date_fin:date
- > rails generate migration AddIdUserToTrips user:references
  > rails db:migrate

J'ai ajouté `has_many :trips` dans le fichier user.rb dans les models

Etape 2

- Création des routes RESTful pour User & trip dans les routes.rb

Generation des controllers :
rails generate controller Trips
rails generate controller Users

Rapport :

Ce que j'ai appris de Ruby on Rails :

1. Framework Web :

Ruby on Rails est un framework web basé sur le langage de programmation Ruby. Il offre une structure prédéfinie pour le développement d'applications web, ce qui facilite la création rapide et efficace de sites web et d'applications.

2. Convention over Configuration (CoC) :

Rails prend décisions par défaut, ce qui simplifie le développement en évitant la configuration manuelle.

3. Don't Repeat Yourself (DRY) :

Rails encourage le principe "Don't Repeat Yourself", incitant à réutiliser du code plutôt que de le dupliquer.

4. MVC Architecture :

L'architecture Modèle-Vue-Contrôleur (MVC) est simple à comprendre pour moi car je connais déjà bien Laravel. Elle sépare la logique de l'application en trois composants, facilitant ainsi la gestion et l'organisation du code.\*

Avantages de Ruby on Rails :

1. Productivité accrue :

Avec Rails le developpement est plus rapide, permettant de créer des fonctionnalités puissantes avec moins de code.

2. Écosystème complet :

Rails offre un écosystème complet avec de nombreux outils, bibliothèques et gems (extensions) disponibles.

3. Communauté active :

Je n'ai pas pu testé mais il semble que la communauté est plutot active.

1. Performance :

Comparé à certains autres frameworks, Rails peut être légèrement moins performant dans certaines situations, bien que des améliorations semble être souvent apportées.

2. Courbe d'apprentissage initiale :

Pour les débutants, la convention peut être étrange au début, et la compréhension complète de la magie interne de Rails peut prendre du temps.

3. Pas idéal pour toutes les applications :

Bien que Rails soit excellent pour les applications web classiques, il peut ne pas être le choix optimal pour des projets nécessitant une architecture plus complexe ou des performances extrêmes.

En tant qu'étudiant, j'apprécie la productivité accrue et la simplicité de développement offertes par Ruby on Rails. Cependant, je suis conscient des compromis potentiels en termes de performance et de courbe d'apprentissage initiale. Globalement, c'est un framework puissant qui trouve son utilité dans de nombreux scénarios de développement web.
