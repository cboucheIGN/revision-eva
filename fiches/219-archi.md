# Architecture informatique

## Réseaux

Un réseau informatique est un ensemble d'équipement réliés entre eux pour échanger des informations.

Indépendamment de la technologie on porte une vue matriciel sur ce qu'est un réseau.

De façon horizontale, un réseau est une strate de trois couches, les infrasctrucutre, les fonctions de controles et de commande et les services rendus à l'utilistaeur.
De façon verticale on utilise souvent un découpage géographique: réseau local, réseau d'accès, réseau d'interconnexion.

### Protocoles

Les applications, outils et services dépendent du type de réseau (Internet, téléphonie, télévision).

Ces types de réseaux implémentent un protocole qui est standardisé (HTTP) ou plutôt une couche de protocole.

![Couches de protocols](https://upload.wikimedia.org/wikipedia/commons/e/e4/TCPIP_couche_ISO_modele_OSI.png?uselang=fr)

### Découpage géographique

- Réseau de la carte mère, le bus informatique
- Réseau local (LAN), relie des ordinateurs situé sur un même site
- Réseau local (WLAN), la même en wifi
- Réseau à grande échelle (WAN)

Références

- Internet
- Intranet
- [Réseau informatique](https://fr.wikipedia.org/wiki/R%C3%A9seau_informatique)
- [DNS](https://fr.wikipedia.org/wiki/Domain_Name_System)

> **Et à l'IGN ?**

Plusieurs réseau, réseau internet d'entreprise, et services web grand public sur internet.

Sur l'intranet on trouve

- les applications support (saisie de congès, rh, documentation, teams, la téléphonie interne)
- la forge logiciel (gitlab, kubernetes)
- les BDDs produit (BDUni)
- services et machine de calcul IA

Pour gérer les applications en exposition public l'IGN passe par son équipe d'exploitation.

Selon la maturité et la complexité du projet peut être sous traité ou à l'inverse pris en charge de manière autonome par la MOA.

GPU est un exemple de projet pour lequel un sous traitant est en charge de l'exploitation

Observatoire des forêts est une projet pour où la MOA est autonome pour l'exploitation (dimensionnement, sécurité, mise à jour)

## Infrastructure programmable

IaC (Infra as Code) est un ensemble de mécanismes permettant de gérer par des fichiers descripteurs ou des scripts une infrastruture virtuelle.

L'évolution des offres dans le domaine de la virtualisation à rendu possible la gstion d'une infrasrcuture à part entière, de l'instance (noeud) au réseau incluant la gestion du DNS, le load balancing, les sous réseau et les groupes de sécurité.

Plébiscité dans le cadre de l'offre cloud computing et de l'approche DevOps. Le but est de répondre au enjeux de mise à l'échelle et la simplification de l'infra.

2006 Amazon dévoile le concept d'IAS permettant le provisionnement d'instance sur un AWS.

Mots clés

- AWS / Microsoft Azure / [Heroku](https://www.heroku.com/)
- Terraform
- Ansible
- load-balancing
- DevOps

> **Et à l'IGN ?**

Plusieurs outils selon les marchés public et technologies associés.

### Ansible - avant 2022

Avant 2022 l'IGN disposait de machine virtuelle auprès de son marché historique.

Les équipes projet documentait leurs script de deploiement puis se dirigait vers des projets Ansible pour gérer plusieurs inventaire de machine (environnement DEV/QUA/PRD) et plusieurs jobs (livraison, dump/restore de BDD, ping)

### Terraform - 2022 le tournant Cloud

Avec le nouveau marché public et le prestataire ovh il a été choisi de migrer les applications exposé au public vers l'offre cloud.

L'équipe sécurité de l'IGN à donc grandi et accueilli des developpeurs mettant en place une infrascture piloté par le code. Elle repose sur une stack d'outil dont terraform pour la gestion des projet et kubernetes pour l'exploitation

Je n'ai jamais pratiqué terraform. On utilise les jobs gitlab pour exploité, les patrons sont fait par équipe MARS.

## Cloud ministériel

Différentes offres cloud ministériel et interministériel, cloud privés de confiance

Les services de l’État et les organismes placés sous sa tutelle doivent dorénavant utiliser le cloud comme modalité d’hébergement par défaut pour leurs projets informatiques, en s’appuyant sur les capacités d’hébergement internes mutualisées de l’État ou sur des fournisseurs privés de confiance.

- [Voir fiche Reglementation](./reglementation.md)
- [numerique.gouv.fr](https://www.numerique.gouv.fr/rechercher/?query=cloud)
- Le Fonds pour la transformation de l’action publique ([FTAP](https://www.numerique.gouv.fr/services/guichet-financement-ftap-adoption-du-cloud-computing/))

> **Et à l'IGN ?**

Mise en marché de cloud privés, ovh cloud remporte le marché
