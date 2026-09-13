# Choix de la politique de sécurité

## 1. Objectif de cette partie

La troisième partie a permis d’évaluer et de hiérarchiser les 15 vulnérabilités relevées lors de l’audit d’ACME Healthcare.

Cinq vulnérabilités ont été retenues comme prioritaires :

1. Les comptes d’anciens employés encore présents ;
2. Les privilèges non autorisés ou excessifs ;
3. Les accès à distance non sécurisés ;
4. Les mots de passe facilement déchiffrables ;
5. Le réseau Wi-Fi utilisant le protocole WEP.

La présente partie consiste à sélectionner un domaine de sécurité à traiter dans la suite du projet et à justifier ce choix à partir des risques identifiés.

Le choix porte sur une politique de **gestion des accès et des habilitations**.

## 2. Politique retenue

La politique retenue est la suivante :

> **Politique de gestion des accès et des habilitations**

Cette politique vise à définir les principes, les règles et les responsabilités permettant de maîtriser les accès des utilisateurs aux systèmes, aux applications, aux équipements et aux informations d’ACME Healthcare.

Elle doit notamment permettre de s’assurer que :

- Chaque accès est attribué à un utilisateur identifié ;
- Les droits accordés correspondent aux fonctions exercées ;
- Les privilèges sont limités au strict nécessaire ;
- Les accès sont supprimés lorsqu’ils ne sont plus justifiés ;
- Les accès sensibles sont contrôlés et révisés ;
- Les mécanismes d’authentification répondent à des exigences de sécurité ;
- Les accès à distance sont soumis à des mesures de protection adaptées.

## 3. Justification du choix

### 3.1 Une politique directement liée aux risques prioritaires

Le choix de la gestion des accès et des habilitations est principalement justifié par la présence de plusieurs vulnérabilités concernant les identités numériques, les comptes utilisateurs et les mécanismes d’accès.

Les comptes d’anciens employés encore présents constituent une faiblesse importante dans le cycle de vie des habilitations.

Les privilèges excessifs montrent également que les droits ne sont pas toujours attribués selon les responsabilités réelles des utilisateurs.

Les mots de passe facilement déchiffrables et les accès à distance non sécurisés concernent quant à eux les mécanismes utilisés pour accéder aux ressources de l’organisation.

Ces vulnérabilités présentent un point commun : elles peuvent permettre à une personne non autorisée d’accéder aux systèmes ou aux informations d’ACME Healthcare.

Une politique de gestion des accès permet donc de traiter une partie importante des risques prioritaires dans un cadre cohérent.

### 3.2 Une politique adaptée au secteur de la santé

ACME Healthcare traite des informations particulièrement sensibles, notamment :

- Des données personnelles concernant les patients ;
- Des informations médicales ;
- Des données administratives ;
- Des informations financières ;
- Des données relatives aux employés.

Dans ce contexte, la maîtrise des accès est essentielle.

Tous les utilisateurs ne doivent pas pouvoir consulter ou modifier l’ensemble des informations disponibles dans le système d’information.

Les droits doivent être attribués en fonction des missions, des responsabilités et du besoin réel d’accès.

Une gestion insuffisante des habilitations pourrait entraîner :

- La consultation non autorisée de données personnelles ou médicales ;
- La modification d’informations sensibles ;
- La divulgation d’informations confidentielles ;
- La compromission de comptes utilisateurs ;
- La difficulté à identifier les responsables d’une opération.

La politique retenue contribue donc directement à la protection de la confidentialité et de l’intégrité des informations.

## 4. Correspondance entre les risques prioritaires et la politique retenue

| Vulnérabilité prioritaire | Lien avec la politique de gestion des accès et des habilitations |
|---|---|
| Comptes d’anciens employés encore présents | La politique doit encadrer la création, la modification, la suspension et la suppression des comptes lors des mouvements du personnel. |
| Privilèges non autorisés ou excessifs | La politique doit imposer le principe du moindre privilège, la validation des droits et la revue périodique des habilitations. |
| Accès à distance non sécurisé | La politique doit définir les conditions d’autorisation des accès distants et exiger l’utilisation de mécanismes sécurisés. |
| Mots de passe facilement déchiffrables | La politique doit intégrer des exigences relatives à l’authentification et à la protection des comptes utilisateurs. |
| Réseau Wi-Fi utilisant le protocole WEP | La politique doit encadrer les conditions d’accès au réseau sans fil et exiger l’utilisation de mécanismes de sécurité adaptés. |

Les deux premières vulnérabilités sont directement couvertes par la gestion des accès et des habilitations.

Les trois autres concernent également des mécanismes techniques spécifiques. Elles seront prises en compte dans la politique à travers des exigences générales de sécurisation de l’authentification, des accès distants et des accès au réseau.

Les mesures techniques détaillées pourront être précisées dans des procédures ou dans des politiques complémentaires.

## 5. Principes de sécurité associés

La politique retenue reposera notamment sur les principes suivants.

### 5.1 Principe du moindre privilège

Chaque utilisateur doit disposer uniquement des droits nécessaires à l’exercice de ses fonctions.

L’attribution de privilèges supplémentaires doit être justifiée, autorisée et tracée.

### 5.2 Principe du besoin d’en connaître

L’accès à une information doit être accordé uniquement lorsque cet accès est nécessaire à l’activité professionnelle de l’utilisateur.

Ce principe est particulièrement important pour les données personnelles et médicales.

### 5.3 Principe de responsabilité individuelle

Chaque utilisateur doit disposer d’un compte individuel permettant d’identifier les opérations réalisées.

Le partage de comptes doit être limité et soumis à des conditions particulières lorsqu’il est indispensable.

### 5.4 Principe du cycle de vie des habilitations

Les droits doivent être gérés pendant toute la durée de vie du compte :

- Création lors de l’arrivée du collaborateur ;
- Modification lors d’un changement de fonction ;
- Révision périodique ;
- Suspension ou suppression lors du départ ;
- Traçabilité des opérations réalisées.

### 5.5 Principe de séparation des responsabilités

Les opérations sensibles doivent, lorsque cela est nécessaire, être réparties entre plusieurs personnes afin de limiter les risques d’erreur, d’abus ou de fraude.

### 5.6 Principe de traçabilité

Les demandes, validations, modifications et suppressions d’habilitations doivent être documentées afin de permettre leur suivi et leur contrôle.

## 6. Périmètre de la politique

La politique s’appliquera notamment aux :

- Collaborateurs d’ACME Healthcare ;
- Prestataires et intervenants externes ;
- Administrateurs systèmes et réseaux ;
- Comptes utilisateurs ;
- Comptes privilégiés ;
- Applications métiers ;
- Bases de données ;
- Systèmes internes ;
- Accès distants ;
- Réseaux sans fil ;
- Ressources contenant des informations sensibles.

Elle concernera les accès physiques et logiques lorsque ceux-ci ont une incidence sur la protection des systèmes d’information.

## 7. Responsabilités concernées

La mise en œuvre de cette politique nécessitera la participation de plusieurs acteurs.

### RSSI

Le RSSI définit les exigences de sécurité, supervise leur application et veille à la cohérence globale de la politique.

### Direction

La direction valide la politique, fournit les moyens nécessaires et soutient son application au sein de l’organisation.

### Ressources humaines

Les ressources humaines transmettent les informations relatives aux arrivées, aux changements de fonction et aux départs des collaborateurs.

### Responsables métiers

Les responsables métiers valident les besoins d’accès des utilisateurs de leur périmètre.

### Équipe informatique

L’équipe informatique met en œuvre les habilitations, applique les changements autorisés et assure la gestion technique des comptes.

### Utilisateurs

Les utilisateurs respectent les règles d’accès, protègent leurs identifiants et signalent toute situation inhabituelle.

## 8. Limites du choix retenu

La politique de gestion des accès et des habilitations ne permet pas, à elle seule, de traiter l’ensemble des vulnérabilités identifiées dans l’audit.

Certaines faiblesses nécessitent également des mesures spécifiques concernant :

- La gestion des correctifs ;
- Le chiffrement des données ;
- La sécurité des réseaux sans fil ;
- La configuration des pare-feu ;
- La supervision et l’analyse des journaux ;
- La sécurisation des postes et des serveurs.

Cependant, la gestion des accès constitue un domaine prioritaire et transversal. Elle permet de formaliser des règles applicables à de nombreux systèmes et utilisateurs, tout en répondant directement à plusieurs risques critiques.

Les autres domaines pourront être traités ultérieurement dans le cadre d’un programme global de sécurité.

## 9. Conclusion

La politique de gestion des accès et des habilitations est retenue en raison de son lien direct avec plusieurs vulnérabilités prioritaires identifiées chez ACME Healthcare.

Elle permet de répondre notamment aux problèmes liés :

- Aux comptes d’anciens employés ;
- Aux privilèges excessifs ;
- À la maîtrise des comptes utilisateurs ;
- À la sécurisation des mécanismes d’authentification ;
- Au contrôle des accès distants et réseau.

Ce choix est également adapté au secteur de la santé, dans lequel la confidentialité, l’intégrité et la traçabilité des informations constituent des enjeux majeurs.

La prochaine partie consistera à rédiger la politique de gestion des accès et des habilitations. Elle précisera les règles de sécurité, les exigences applicables, les responsabilités et les principes que les utilisateurs et les équipes techniques devront respecter.
