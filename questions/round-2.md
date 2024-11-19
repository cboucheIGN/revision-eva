# Round 2

## Méthode impact

> Parlez de la méthodologie par impact

- [Méthode des Piliers d’impact](https://www.digilityx.com/post/methode-des-piliers-dimpact)

## Refonte

> La MOA vous demande la refonte d'un produit que lui proposez vous ?

Ici produit désignera un service web pour lequel la MOE à la responsablité de développé les outils, déploiyer le service sur internet et de maintenir en condition opérationnelle (correction de bugs)

On se mettra d'accord pour qu'il n'y ai pas de perte fonctionnelles (refonte graphique ou fonctionnelle, tehcnique).

MOA / MOE

Refonte ? Une refonte est différente d'un évolution fonctionnelle dans le sens où tout le système ou une partie non négligeble est modifié. (Cela suppose qu'on change le moule). Cela implique qu'une partie du code sera considéré comme obsolète / deprecated.

La refonte est motivé par quoi ?

- Refonte technique
  - changement de prestataire dans le cadre d'un renouvellement de marché public
  - migration de piwik vers matomo
  - migration vers le cloud, alors il a fallu revoir l'architecture et le déploiement des sites
- Recyclage - le produit n'est plus pérenne ou financé, alors il s'agit de garder les bonnes idées et de faire évolué le parcours utilisateur vers un nouveau besoin identifié
  - le produit Mon-Geoportail etait mis de côté car pas assez de nouveaux partenaires pour justifié une approche systèmique et autonomisante. Alors extraction du service et transformation en librairie **geoportal-client**
- Refonte graphique - un changement de design
  - le site **observatoire des forets** va migrer depuis le design systeme IGN vers le design system DSFR.
- Refonte fonctionnelle - différence avec évolution fonctionnelle ?
  - Par exemple l'outil OVACARTE à été refondue dans le produit espace collaboratif.

Pour confort de la discussion on appelera V1 la version existante du produit, et V2 la version après refonte.

Je lui propose de mesurer les impacts du changement. Ensuite je les accompagne pour définir la liste des changements. Il est possible que le changement soit arbitré par les coût de changer (donc pré-analyse à faire).

La liste des changements définiront un nouveau backlog sur lequel on estime le temps de DEV et l'impact sur l'utilisateur final (afin de sortir une V2 de haute valeur ajouté le plus rapidement possible).

On priorise les changements et on les traites du plus impactant jusqu'au finition.

Méthode produit

Rappel méthode produit.

On intégre les changement dans le nouveau cycle de sprint. A chaque sprint on livre la nouvelle version dans l'environnement de DEV. Sur l'espace de DEV sera fait la recette.

L'environnement de PROD sera toujours sur la V1 jusqu'à mise en place d'un plan de communication pour faire passer les utilisateurs à la V2. Il faudra prévoir des formations / webinaire / présentation pour accompagner le changement.

Une refonte peux induire une évolution du modèle de données. Par exemple lors la migration vers le DSFR il a fallu modifier la façon de stocké l'éditorial dans une BDD. Alors il a fallu définir des script de migration afin de pouvoir passé d'une BDD compatible avec l'application v1 vers une BDDv2 compatible avec le nouveau produit.
