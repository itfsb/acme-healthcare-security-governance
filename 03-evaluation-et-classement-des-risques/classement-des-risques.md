## 4. Registre des risques

Les cotations suivantes sont établies à partir des informations du scénario. Elles constituent des estimations qualitatives destinées à comparer les vulnérabilités entre elles.

| ID | Vulnérabilité | Actif ou processus concerné | Menace ou scénario d’exploitation | Vraisemblance | Impact | Score | Niveau |
|---|---|---|---|---:|---:|---:|---|
| R01 | Comptes d’anciens employés encore présents | Comptes utilisateurs et systèmes internes | Utilisation d’un ancien compte après le départ d’un collaborateur. | 5 | 5 | 25 | Critique |
| R02 | Privilèges non autorisés ou excessifs | Habilitations, applications et bases de données | Exploitation de droits supérieurs à ceux nécessaires aux fonctions. | 4 | 5 | 20 | Critique |
| R03 | Accès à distance non sécurisé | Accès distants, télétravail et systèmes exposés | Interception, détournement ou exploitation d’un accès distant insuffisamment protégé. | 4 | 5 | 20 | Critique |
| R04 | Mots de passe facilement déchiffrables | Authentification et comptes utilisateurs | Récupération ou devinage rapide de mots de passe faibles. | 5 | 5 | 25 | Critique |
| R05 | Expiration des mots de passe non standardisée | Politique d’authentification | Conservation de mots de passe anciens pendant des durées variables. | 3 | 3 | 9 | Modéré |
| R06 | Fichiers sensibles non chiffrés sur les terminaux | Postes de travail et fichiers locaux | Accès à des fichiers après perte, vol ou compromission d’un terminal. | 3 | 5 | 15 | Élevé |
| R07 | Réseau Wi-Fi utilisant le protocole WEP | Réseau sans fil | Exploitation des faiblesses de WEP pour accéder au réseau interne. | 4 | 4 | 16 | Élevé |
| R08 | E-mails sensibles non chiffrés | Messagerie et échanges avec l’extérieur | Interception d’informations sensibles lors d’un échange externe. | 3 | 5 | 15 | Élevé |
| R09 | Journaux IDS rarement examinés | Supervision, détection et réponse aux incidents | Activité malveillante détectée mais non analysée à temps. | 3 | 4 | 12 | Élevé |
| R10 | Équipements contenant des données sensibles utilisés à titre privé | Terminaux professionnels et données locales | Utilisation privée d’un équipement contenant des données sensibles. | 3 | 4 | 12 | Élevé |
| R11 | Postes laissés sans surveillance et sessions ouvertes | Postes de travail et sessions utilisateurs | Utilisation d’une session restée ouverte par une personne non autorisée. | 3 | 4 | 12 | Élevé |
| R12 | Mises à jour et configurations incohérentes | Postes, serveurs et équipements réseau | Exploitation d’un équipement insuffisamment mis à jour ou mal configuré. | 3 | 4 | 12 | Élevé |
| R13 | Pare-feu autorisant tout sauf refus explicite | Filtrage réseau et pare-feu | Autorisation d’un flux inutile ou malveillant non explicitement bloqué. | 3 | 4 | 12 | Élevé |
| R14 | Serveurs non corrigés | Serveurs et services applicatifs | Exploitation d’une vulnérabilité connue sur un serveur non corrigé. | 3 | 5 | 15 | Élevé |
| R15 | Intranet permettant de modifier des informations personnelles | Intranet, applications et bases de données | Modification d’informations personnelles sans contrôle suffisant. | 3 | 4 | 12 | Élevé |

## 5. Classement des risques

Le classement est réalisé à partir du score obtenu pour chaque risque.

Lorsque plusieurs risques obtiennent le même score, ils sont départagés selon leur ordre d’apparition dans le registre afin d’obtenir un rang unique.

| Rang | ID | Vulnérabilité | Score | Niveau |
|---:|---|---|---:|---|
| 1 | R01 | Comptes d’anciens employés encore présents | 25 | Critique |
| 2 | R04 | Mots de passe facilement déchiffrables | 25 | Critique |
| 3 | R02 | Privilèges non autorisés ou excessifs | 20 | Critique |
| 4 | R03 | Accès à distance non sécurisé | 20 | Critique |
| 5 | R07 | Réseau Wi-Fi utilisant le protocole WEP | 16 | Élevé |
| 6 | R06 | Fichiers sensibles non chiffrés sur les terminaux | 15 | Élevé |
| 7 | R08 | E-mails sensibles non chiffrés | 15 | Élevé |
| 8 | R14 | Serveurs non corrigés | 15 | Élevé |
| 9 | R09 | Journaux IDS rarement examinés | 12 | Élevé |
| 10 | R10 | Équipements contenant des données sensibles utilisés à titre privé | 12 | Élevé |
| 11 | R11 | Postes laissés sans surveillance et sessions ouvertes | 12 | Élevé |
| 12 | R12 | Mises à jour et configurations incohérentes | 12 | Élevé |
| 13 | R13 | Pare-feu autorisant tout sauf refus explicite | 12 | Élevé |
| 14 | R15 | Intranet permettant de modifier des informations personnelles | 12 | Élevé |
| 15 | R05 | Expiration des mots de passe non standardisée | 9 | Modéré |

## 6. Analyse du classement

L’évaluation fait apparaître quatre risques critiques :

- Les comptes d’anciens employés encore présents ;
- Les mots de passe facilement déchiffrables ;
- Les privilèges non autorisés ou excessifs ;
- Les accès à distance non sécurisés.

Ces risques concernent directement la maîtrise des identités, des authentifications et des accès aux systèmes d’information. Leur exploitation pourrait permettre à une personne non autorisée d’accéder à des ressources internes ou à des informations sensibles.

Le réseau Wi-Fi utilisant WEP présente également un niveau de risque élevé. Le caractère obsolète de ce protocole facilite les tentatives d’accès non autorisé au réseau et justifie son traitement prioritaire.

Les autres vulnérabilités présentent également des niveaux de risque importants. Elles devront être prises en compte dans une démarche globale de sécurité, mais elles ne constituent pas le périmètre principal de la politique développée dans la suite du projet.

## 7. Sélection des vulnérabilités prioritaires

À l’issue de l’évaluation, cinq vulnérabilités sont retenues pour faire l’objet d’un approfondissement dans la suite du projet :

1. Les comptes d’anciens employés encore présents ;
2. Les privilèges non autorisés ou excessifs ;
3. Les accès à distance non sécurisés ;
4. Les mots de passe facilement déchiffrables ;
5. Le réseau Wi-Fi utilisant le protocole WEP.

Cette sélection correspond aux cinq premières positions du classement.

Elle repose sur les critères suivants :

- Le niveau de risque estimé ;
- La sensibilité des systèmes et des informations concernés ;
- La facilité potentielle d’exploitation ;
- Le caractère transversal des vulnérabilités ;
- La possibilité de formaliser des règles de sécurité ;
- La possibilité de définir des responsabilités et une procédure opérationnelle.

Les autres vulnérabilités ne sont pas considérées comme négligeables. Elles devront faire l’objet d’actions complémentaires dans le cadre d’un programme global de sécurité.

## 8. Résultat de l’évaluation

L’analyse met en évidence une exposition importante d’ACME Healthcare aux risques d’accès non autorisé, de compromission des systèmes et de divulgation d’informations sensibles.

Les cinq vulnérabilités retenues constituent un périmètre cohérent pour la suite du projet, car elles concernent principalement :

- La gestion des comptes utilisateurs ;
- La maîtrise des privilèges ;
- La sécurisation des accès distants ;
- La robustesse de l’authentification ;
- La sécurité des réseaux sans fil.

La prochaine partie consistera à choisir et à justifier le domaine de politique de sécurité à développer à partir de ces cinq vulnérabilités prioritaires.
