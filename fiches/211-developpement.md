# Developpement

Le développement de logiciel consiste à étudier, concevoir, construire, transformer, mettre au point, maintenir et améliorer des logiciels.

Il comprend plusieurs étapes. Le séquencage dépendra de la méthode projet utilisé.

- L'analyse est le recessement et la documentation de chaque fonctionnalités
- La conception est la déterminiation des solutions techniques
- La construction est la principale activité qui consiste en la redaction du code source
- La recette assure par des contrôles la qualité du produit

> **Et à l'IGN ?**

Poste de Concepteur développeur / Responsable de développement.

60% du temps consiste à développer les services informatique. Principalement des sites webs.

Une stack pour développer un site web comprend

- Un langage de programmation ([HTML](https://developer.mozilla.org/fr/docs/Web/HTML)/[CSS](https://developer.mozilla.org/fr/docs/Web/CSS)/[Javascript](https://developer.mozilla.org/fr/docs/Web/JavaScript))
- Un framework côté client ([Angular](https://angular.dev/))
- Un ensemble de librairie libres ([Openlayer](https://openlayers.org/), DSFR)
- Un framework côté serveur ([express](https://expressjs.com/) / [Symfony](https://symfony.com/))
- Un outil de virtualisation des deploiement [docker](https://www.docker.com/)
- Un projet [kubernetes](https://kubernetes.io/) permettant de déployer les images dans le cloud ([Helm](https://helm.sh/))

L'agent intervient à tous ces niveaux en respectant les bonnes pratiques et recommandations.

## Notion de programmation : algorithme, mode de représentation

L'algorithmique est l'étude et la production de règles et techniques qui sont impliquées dans la définition et la conception d'algorithmes, c'est-à-dire de processus systématiques de résolution d'un problème permettant de décrire précisément des étapes pour résoudre un problème algorithmique.

Références

- [Algorithmique](https://fr.wikipedia.org/wiki/Algorithmique)
- [https://fr.wikipedia.org/wiki/Structure_de_donn%C3%A9es](https://fr.wikipedia.org/wiki/Structure_de_donn%C3%A9es)

> **Et à l'IGN ?**

## notions d'UX et UI

L'expérience utilisateur (UX) est la qualité du vécu de l'utilisateur dans des environnements numériques ou physiques. C'est une notion de plus en plus courante là où l'on utilisait, encore récemment, les notions d'ergonomie des logiciels et d'utilisabilité.

Références

- [Expérience utilisateur](https://fr.wikipedia.org/wiki/Exp%C3%A9rience_utilisateur)
- [Interface utilisateur](https://fr.wikipedia.org/wiki/Interface_utilisateur)

> **Et à l'IGN ?**

## Organisation des travaux de programmation

Références

- [cf projet](./217-projet.md)

> **Et à l'IGN ?**

## code : infrastructure codée, code applicatif, code test automatisée

Références

- [Infrasturure as Code - cf archi](./219-archi.md)
- [Orchestrateur de deploiement - Jenkins](https://www.jenkins.io/)

> **Et à l'IGN ?**

IaS. Ajout de contrainte pour miniser/maitriser les risques informatique. Par exemple une image ne sera pas éxécuter avec un compte qui à des droits en écriture sur le systeme, et qui ne se saurait être élévé au rang admin.

## outils et environnements de développement : éditeur, compilateur, environnements d'exécutions, qualité du code, outils d'analyse du code, outils d'aide à la programmation

### Code coverage

En génie logiciel, la couverture de code est une mesure utilisée pour décrire le taux de code source exécuté d'un programme quand une suite de test est lancée. Un programme avec une haute couverture de code, mesurée en pourcentage, a davantage de code exécuté durant les tests ce qui laisse à penser qu'il a moins de chance de contenir de bugs logiciels non détectés, comparativement à un programme avec une faible couverture de code1,2. Différentes métriques peuvent être utilisées pour calculer la couverture de code ; les plus basiques sont le pourcentage de sous routine et le pourcentage d'instructions appelées durant l'exécution de la suite de test.

Références

- [Visual studio code](https://code.visualstudio.com/)
- [Environnement d'execution - Firefox]
- [Qualité de code - sonarcube](https://www.sonarsource.com/solutions/clean-code/)
- [Comment analyser la qualité de votre code](https://www.troispointzero.fr/le-blog/sonarqube/)
- [Code coverage](https://fr.wikipedia.org/wiki/Couverture_de_code)
- [Détection automatique de vulnérabilité - Renovate](https://docs.renovatebot.com/)

> **Et à l'IGN ?**

## les tests : les différents types de tests : Unitaires, tests automatisés (Test Driven Development)

### Test unitaire

En programmation informatique, le test unitaire (ou « T.U. », ou « U.T. » en anglais) est une procédure permettant de vérifier le bon fonctionnement d'une partie précise d'un logiciel ou d'une portion d'un programme (appelée « unité » ou « module »).

La méthode XP préconise d'écrire les tests en même temps, ou même avant la fonction à tester ([Test Driven Development](https://fr.wikipedia.org/wiki/Test_driven_development)). Ceci permet de définir précisément l'interface du module à développer. Les tests sont exécutés durant tout le développement, permettant de visualiser si le code fraîchement écrit correspond au besoin.

Les tests unitaires peuvent servir de complément à l'API, il est très utile de lire les tests pour comprendre comment s'utilise une méthode. De plus, il est possible que la documentation ne soit plus à jour, mais les tests eux correspondent à la réalité de l'application.

On définit généralement 4 phases dans l'exécution d'un test unitaire :

- Initialisation (fonction setUp) : définition d'un environnement de test complètement reproductible (une fixture).
- Exercice : le module à tester est exécuté.
- Vérification (utilisation de fonctions assert) : comparaison des résultats obtenus avec un vecteur de résultat défini. Ces tests définissent le résultat du test : SUCCÈS (SUCCESS) ou ÉCHEC (FAILURE). On peut également définir d'autres résultats comme ÉVITÉ (SKIPPED).
- Désactivation (fonction tearDown) : désinstallation des fixtures pour retrouver l'état initial du système, dans le but de ne pas polluer les tests suivants. Tous les tests doivent être indépendants et reproductibles unitairement (quand exécutés seuls).

Références

- [Test unitaire](https://fr.wikipedia.org/wiki/Test_unitaire)
- [Test unitaire - Karma](https://karma-runner.github.io/latest/index.html)
- [Test unitaire - Junit](https://junit.org/junit5/)
- [Réalisez des tests End-to-End](https://openclassrooms.com/fr/courses/7159306-testez-vos-applications-front-end-avec-javascript/7332824-realisez-des-tests-end-to-end)
- [Test e2e - Cypress](https://docs.cypress.io/app/get-started/why-cypress)

> **Et à l'IGN ?**
