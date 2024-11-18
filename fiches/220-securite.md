# Notions générales sur la sécurite informatique

## ANSSI - Agence nationale de la sécurité des systèmes d'information

Créée en 2009, l’Agence nationale de la sécurité des systèmes d'information (ANSSI) est l'autorité nationale en matière de cybersécurité. Sa mission est de comprendre, prévenir et répondre au risque cyber.

[Rapport d'activité 2023](https://cyber.gouv.fr/sites/default/files/document/Rapport%20d%27activit%C3%A9%202023%20de%20l%27ANSSI.pdf)

Les missions

- Défendre
  - les systèmes d'information critiques de la Nation en concevant et opérant de capacités de détection des cyberattaques
  - les victimes des cyberattaques
  - la nation en structurant au niveau national l'assistance aux victimes de cyberattaques
- Connaitre
  - l'état de l'art et en être expert
  - les menaces et développé les outils pour detecter et prévenir
  - les référentiels européens, internationnale et s'inscrire dans une démarche de protection du cyberespace
- Partager
  - des recommandation de cybersécurité
  - les solutions
  - l'expertise
- Accompagner
  - l'état dans la création d'une doctrine française de sécurité
  - le développement d'un ecosysteme de prestataires et produits de confiance

> **Et à l'IGN ?**

Initiative de l'équipe MARS - Inscription au challenge SSI IGN 2023 voir mail 22/03/2023

## L'homologation des SI grand public

[L'homologation de sécurité](https://cyber.gouv.fr/lhomologation-de-securite) permet à un responsable de s'informer et attester aux utilisateurs que les risques qui pèsent sur eux sont connu et maitrisé.

D'autant plus nécessaire qu'une attaque ou une interuption de service sont de plus en plus grave à mesure que les SI se complexifient

Rendu obligatoire par des textes pour de nombreux SI

- [IGI 1300](https://cyber.gouv.fr/instruction-generale-interministerielle-n1300) - l’Instruction générale interministérielle no 1300
- RGS - le référentiel général de sécurité
- PSSIE - la politique des système d'information de l'état

En informatique, comme dans d’autres domaines, le risque zéro n’existe pas.

ANSSI accompagne les homologations avec [MonServiceSécusé](https://monservicesecurise.cyber.gouv.fr/)

> **Et à l'IGN ?**

La mission MARS demande et accompagne les agents à plusieurs étapes du projet, au début pour valider l'architecture et choisir les solutions adaptés et sécurisé.

Elle invite les responsable MOA / d'application à remplir le dossier d'homologation. Anciennement elle demandait à remplir une PSSI.

Les agents responsable de dev sont abonné à la newsleter de MonServiceSécurisé

Une homologation de sécurité est à assuré en vue de besoin de sécurité et d'une mesure des risques d'attaque ou perte.

Dans un DAT on définit une matrice d'exigence, elle permettra de cibler le niveau d'infogérence et de contrôle à mettre en place.

| Exigence                                                     | Niveau |
|--------------------------------------------------------------|--------|
| Disponibilité                                                | D2 - Moyen: Ce niveau traduit un délai maximal d'interruption d'une semaine. Un système s'interrompant le mercredi sera rétabli au plus tard le mardi dans la journée ouvrée. |
| Intégrité                                                    | I1 - Faible: Il est nécessaire de savoir détecter les erreurs significatives, mais sans garantie d’exhaustivité |
| Confidentialité                                              | C1 - Inexistant - Public |
| Traçabilité                                                  | T1 - Faible: Traçabilité des actions |
| Performance                                                  | P1 - Exigence faible. Le système vise à une performance définie, sans que la non-tenue de cette exigence soit très dommageable à l'IGN. |
| Élasticité                                                   | E1: Le service doit être en mesure de faire face à des pics de charge planifiés suffisamment à l'avance. |
| Plage horaire d'utilisation du service                       | 24/7 |
| Plage horaire nécessitant un niveau de disponibilité garanti | 5/7 9:30-16:00 |
| Perte de Données Maximale Autorisée (PDMA)                   | S2 - PDMA >= une semaine: la perte des données est acceptable jusqu'à une amplitude d'une semaine |
| Engagements de Maintien en condition Opérationnel            | 1 mois |

Référence

- [DAT GPE](https://gitlab.ign.fr/dat/ignmut/foreg/-/blob/main/SP_DAT-GPE.md)

## DevSecOps

L'approche DevSecOps (Development - Security - Operations) est une approche qui permet d'intégrer la sécurité des données dès le début d'un projet. La sécurité de celles-ci est considérée comme une condition préalable avant de commencer.

Historiquement les processus liés à la sécurité étaient isolés et attribués à un groupe spécifique lors de la phase finale de développement.

Avec une approche DevOps assurants des livraisons rapides et fréquente les méthodes de sécurité doivent évolué.

Voir [la fiche DevOps](./devops.md)

- [Qu'est-ce que l’approche DevSecOps ?](https://www.oracle.com/fr/security/definition-approche-dev-sec-ops/)

> **Et à l'IGN ?**

## VPN

Un VPN d'entreprise est un réseau privé virtuel conçu pour les entreprises. Il permet aux travailleurs à distance d'accéder en toute sécurité aux réseaux internes ou à l'intranet d'une entreprise, et il peut être utilisé pour créer un réseau partagé unique entre les travailleurs et les différents sièges. L'objectif principal d'un VPN d'entreprise est d'empêcher que les données internes et le trafic Internet propriétaire ne soient divulgués au monde entier (et, par extension, aux pirates informatiques et aux cybercriminels).

- [What is VPN](https://www.kaspersky.fr/resource-center/definitions/what-is-business-vpn)

> **Et à l'IGN ?**

le client VPN BigIP sécurisé par mot de passe personnel, changé une fois pas an.

## A surveiller

nouvelle réglementation NIS2 européen

## Secure by design

l'approche secure by design défendue à l'IGN

- integrer gestion de projet (user story et evil user story "je me met en position d'attaquant")
- pas de sécurité post déploiement
- minimiser la surface d'attaque
- principe de moindre privilege
- securité tous les niveaux
- detection d'intrusion
- ne pas faire confiance
- séparer les respon
- gérer un backlog des risques

Renovbot / SBOM cycle mdx
- les systemes sont complexes
- format de répresentation des dépendances
- détéction de secret dans les dépot (bloque le commit)
