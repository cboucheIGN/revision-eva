# Notion en méthode de conduite de projets

## Cycle en V

Le cycle en V est un modèle d'organisation des activités d'un projet qui se caractèrise par un flux d'activé descendant qui détaille le produit jusqu'à sa réalisation, et un flux ascendant qui assemble le produit en vérifiant sa qualité. Issue du modèle en cascade dont il reprend l'approche séquentielle et linéaire des phases

Issue du monde de l'industrie il devient un standard dans l'indutrie du logiciel depuis les années 80.

Dans le flux descendant on vise à détailler le produit jusqu'à sa réalisation. Il comprend

- l'expression des besoins
- l'analyse
- la conception
- la mise en oeuvre (la programmation)

Dans le flux ascendant on vise à valider le produit jusqu'à sa recette, c'est à dire son acceptation par le client. (série de tests).

Le cycle en V comporte la notion de système, le produit du projet en considèré comme un système fait de plusieurs éléments qui sont des modules ou composants. Ceci requiert dans le flux descendant de décrire indépendamment chaque modules.

Le cycle en V fait la belle part au test: test unitaire (robuste), test d'intégration (deployable), test de validation système (conforme au exigence).

Dans ce système on retrouve les roles suivants

- MOA Maitrise d'ouvrage qui regroupe toutes les fonction suivante
  - la stratégie
  - l'opérationnel
  - les experts métiers
  - les utilisateurs
- MOE Matrise d'oeuvre
  - l'équipe architecturale
  - l'équipe de développement
  - le titutaire du marché
- Le comité de pilotage améliore le suivi du projet et à l'autorité pour faire des choix et trancher des conflits

Dans le cycle en V les roles sont appelé à chaque étape du projet (on ne trouve pas les développeur au niveau de la description fonctionnelle, ni la MOA pendant la définition des test unitaires)

![Cycle en V](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Systems_Engineering_Process_II.svg/langfr-450px-Systems_Engineering_Process_II.svg.png)

- [Cycle en V](https://fr.wikipedia.org/wiki/Cycle_en_V)

> **Et à l'IGN ?**

Méthode projet historique permit de conduire des grands projets à l'IGN.

Première expérience à l'IGN garde des traces du cycles en V avec des cahiers de charge, des cahiers de spécifications techniques. Avec une approche mixte en incorporant la méthode agile au maximum. Les COPILS sont toujours présent pour arbitrer les conflits de ressources humaines, prevenir les risques de dérives (calendaire, budgetaire, qualité).

## Agilité : les différentes méthodes agile

Le Manifeste pour le développement agile de logiciels est un texte rédigé aux États-Unis en 2001 par dix-sept experts du développement logiciels. Ils estimaient que le taux important d'échecs des projets de développements logiciels était dû à la lourdeur des méthodes traditionnelles inspirées du génie civil et s'appuyant sur un cycle de développement en cascade

Naissance de la méthode agile suite au constat que bcp de projet industrielle informatique n'était en échec pas contractuellement mais par un écart trop important avec le besoin de l'utilsateur final qui à pu évoluer le temps de la conception et réalisation dans un cycle en v.

### Les méthodes

- RAD (rapid application devloppement) 1991 - 1995
- SCRUM 1995 - 2010
  - Sprint planning
  - burndown chart
  - daily stand-up meeting (daily scrum)
- Extreme programming 1999
- ASD - adaptive sofware develpment (RAD v2)
- FDD 2003 - feature-driven develppement
- BDD 2004 - behavior-driven developpent

A grandes échelles (plusieurs équipes agiles à organisé dans une même entreprises)

- [SAFe](https://fr.wikipedia.org/wiki/Scaled_agile_framework) - scale agile framework
- LeSS - large scale scrum

### Critique

La plus part des projets agiles en 2018 sont "faux-agile" et ne respectent pas ses valeurs et principes. Ainsi les 3 défis

- se battre contre l'industrie agile (qui devient un arguement marketing) et sa tendance à imposer les processuss aux équipes
- insiter sur l'importance de l'excellence technique
- organiser les équipes autour d'un produit et non d'un projet

### Manifeste agile

4 valeurs. Accorder de l'importance à

- aux individus et leurs interactions plutôt qu'aux outils et processus
- à un logiciel fonctionnel plutôt qu'a une documentation exhaustive
- à la collaboration avec les clients plutôt qu'à la négociation contractuelle
- à l'adaptation au changement plutôt qu'à l'execution du plan

12 principces

- notre plus haute priorité est de satisfaire le client en livrant rapidemnt et régulièrement des fonctionnaltiés à grande valeur ajoutée
- Accueuillez positivement les changements de besions, même tard ans le projet. Les processus Agiles exploitent le changement pour donner un avantage compétitif au client.
- Livrez fréquement un logiciel fonctionnel, dans des cycles de quelques semaines à quelques mois, avec une préférence pour les plus court.
- Les utilisateurs ou leurs répsentatn et développeur doivenet travailer ensemble quotidiennement tout au long du projet
- Réalisez les projets avec des personnes motivés. Fournissez leur l'environnement et le soutien dont elles ont besoin et faites leur confiance pour atteindre les objectifs fixés.
- La convesation en face à face est la méthode la plus efficae et économique pour donner des informations à une équipe de réalisation, et pour échanger des informations à l'intérieur de de l'équipe
- La disponibilité de solutions opérationnelles est la principale mesure d'avancement
- les processus agiles encouragent à respecter un tythme soutenable lors de la réalisation. Les commanditaires, les réalisateurs et les utilsateurs devrait pouvoir maintenir indéfiniment un rythme constant.
- Porter continuellement attention à l'excellence technique et à la qualité de la conception renforce l'agilité
- La simplicité - l'art de maximiser la quantité de travail qu'on ne fait pas - est essentielle
- Les meilleures architectures, les meilleurs spécifications de besoins, et les meilleurs conceptions émergenet d'équipe auto-organisés
- a intervalles réguliers, l'équipe réfléchit aux façon de devenir plus efficace puis modifie son comportement et l'ajuste en conséquence.

- [Méthode agile 2001](https://fr.wikipedia.org/wiki/M%C3%A9thode_agile)
- [Manifeste agile](https://fr.wikipedia.org/wiki/Manifeste_agile)
- [Xtreme programming]
- [Scrum](https://fr.wikipedia.org/wiki/Scrum_(d%C3%A9veloppement))
- [SAFe](https://fr.wikipedia.org/wiki/Scaled_agile_framework)

> **Et à l'IGN ?**

La majorité des projets que j'ai mené était sous mode agile. Avec une équipe projet composé

- d'experts métiers (gage que le besoin de l'utilisateur final sera rendu)
- de developpeur (1 à 4 personne selon la charge)
- des designeur (surtout dans les phases de pré-développement)
- d'ingénieur projet garant des horloges, pilotant l'équipe

Les valeurs agiles sont plutôt bien respecté car une grande autonomie est donnée à l'équipe projet. Elle s'engage également dans un processus de dialogue avec le porteur de projet et les utilistaeurs finaux.

On reçois régulièrement (lors des points dev) de nouvelles commandes permettant de préciser, d'améliorer l'expérience utilsiateur.

## Mode produit

Le mode produit est une méthodologie de travail qui consiste à se focaliser sur la valeur apportée à son client et aux utilisateurs finaux. Le produit se construit au fur et à mesure de manière itérative en prenant en compte les feedbacks utilisateurs afin de l’améliorer constamment.

En opposition au mode projet où l’on pilote avec les enveloppes budgétaires, le mode produit amène le pilotage par la valeur. On priorise les projets par la valeur, on définit le ROI (retour sur investissement) possible, et on priorise les actions à faire en fonction de la valeur business apportée, donc du plus gros ROI.

Quel que soit le format de solution cloud choisi, le mode produit doit être privilégié. Il inclut :

- l’autonomie des équipes
- la prise en charge continue des opérations
- la confrontation rapide avec les utilisateurs du produit
- un jalonnement par l’impact permettant d’arrêter, d’infléchir ou d’accélérer la trajectoire du produit en fonction des résultats constatés.

- [Le Cloud pour les administrations](https://www.numerique.gouv.fr/services/cloud/faq/)
- [Mode projet vs mode produit](https://www.reussirsesprojets.com/mode-projet-vs-mode-produit/#t-1658230401569)

> **Et à l'IGN ?**

Nouvelle méthode mise en avant à l'IGN

## Les outils et indicateurs, mesures de performance
