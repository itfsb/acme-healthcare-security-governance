# Analyse des vulnérabilités

## 1. Objectif de l’analyse

L’audit réalisé chez ACME Healthcare a permis d’identifier plusieurs faiblesses dans les systèmes d’information et dans les pratiques de sécurité.

Cette partie consiste à examiner les 15 constats relevés lors de l’audit afin de comprendre :

- La nature de chaque vulnérabilité ;
- Les ressources ou processus concernés ;
- La faiblesse observée ;
- La manière dont cette faiblesse pourrait être exploitée ;
- Les conséquences possibles pour l’organisation.

Cette analyse reste descriptive. L’évaluation de la probabilité, de l’impact et du niveau de risque sera réalisée dans la troisième partie.

## 2. Méthode d’analyse

Chaque vulnérabilité est présentée selon les éléments suivants :

| Élément | Description |
|---|---|
| Constat | Faiblesse relevée lors de l’audit |
| Domaine concerné | Système, processus ou pratique concerné |
| Description | Explication de la faiblesse observée |
| Exploitation possible | Manière dont la faiblesse pourrait être utilisée |
| Conséquences possibles | Effets que cette exploitation pourrait produire |

Les conséquences présentées ne constituent pas encore une évaluation du risque. Elles servent à comprendre les enjeux associés à chaque vulnérabilité.

## 3. Analyse des vulnérabilités identifiées

### 3.1. Comptes d’anciens employés toujours actifs

**Constat :**  
Des comptes appartenant à d’anciens employés sont toujours présents dans les systèmes d’information.

**Domaine concerné :**  
Gestion des comptes et des accès.

**Description :**  
Les comptes utilisateurs ne sont pas systématiquement désactivés ou supprimés lors du départ d’un collaborateur.

Cette situation signifie que certains comptes peuvent continuer à exister alors que leurs propriétaires ne travaillent plus pour l’organisation.

**Exploitation possible :**

- Utilisation d’identifiants encore valides ;
- Réutilisation d’un compte par une autre personne ;
- Compromission d’un ancien compte ;
- Accès à des applications ou à des ressources internes.

**Conséquences possibles :**

- Accès à des informations sans autorisation ;
- Utilisation d’une identité qui ne devrait plus être active ;
- Difficulté à identifier l’auteur réel d’une action ;
- Maintien d’un accès après la fin de la relation professionnelle.

### 3.2. Privilèges excessifs ou non autorisés

**Constat :**  
Certains utilisateurs disposent de privilèges supérieurs à ceux nécessaires à leurs fonctions.

**Domaine concerné :**  
Gestion des habilitations et contrôle des accès.

**Description :**  
Les droits attribués aux utilisateurs ne correspondent pas toujours à leurs responsabilités réelles.

Certains comptes peuvent ainsi accéder à des ressources, effectuer des opérations ou modifier des informations qui ne sont pas nécessaires à leur activité.

**Exploitation possible :**

- Utilisation abusive de droits existants ;
- Exploitation d’un compte compromis ;
- Consultation de ressources non nécessaires ;
- Modification ou suppression d’informations.

**Conséquences possibles :**

- Accès à des données confidentielles ;
- Modification non autorisée de données ;
- Suppression accidentelle ou volontaire d’informations ;
- Extension des conséquences d’une compromission de compte.

### 3.3. Accès à distance non sécurisé

**Constat :**  
Les accès à distance aux ressources de l’organisation ne sont pas suffisamment sécurisés.

**Domaine concerné :**  
Accès distant et télétravail.

**Description :**  
Les connexions établies depuis l’extérieur peuvent ne pas bénéficier de contrôles suffisants concernant l’authentification, le chiffrement ou la surveillance.

Les utilisateurs peuvent également se connecter depuis des réseaux ou des équipements qui ne présentent pas le même niveau de sécurité que le réseau interne.

**Exploitation possible :**

- Interception de communications ;
- Vol d’identifiants ;
- Utilisation d’un poste distant compromis ;
- Connexion frauduleuse à un service accessible depuis Internet.

**Conséquences possibles :**

- Accès non autorisé au réseau interne ;
- Consultation de ressources internes ;
- Compromission de comptes ;
- Transmission ou extraction de données.

### 3.4. Mots de passe facilement déchiffrables

**Constat :**  
Environ 40 % des mots de passe peuvent être déchiffrés en six heures.

**Domaine concerné :**  
Authentification et protection des comptes.

**Description :**  
Une partie des mots de passe utilisés par les comptes de l’organisation ne présente pas une résistance suffisante face aux techniques de récupération ou de déchiffrement.

Cette situation peut être liée à des mots de passe faibles, réutilisés ou à des mécanismes de stockage insuffisamment protégés.

**Exploitation possible :**

- Attaque par force brute ;
- Attaque par dictionnaire ;
- Utilisation de mots de passe récupérés ;
- Réutilisation d’identifiants sur plusieurs services.

**Conséquences possibles :**

- Prise de contrôle de comptes ;
- Accès à des applications internes ;
- Usurpation d’identité ;
- Utilisation d’un compte compromis pour accéder à d’autres ressources.

### 3.5. Expiration des mots de passe non standardisée

**Constat :**  
Les règles d’expiration des mots de passe ne sont pas uniformes selon les systèmes.

**Domaine concerné :**  
Politique d’authentification.

**Description :**  
Les différents systèmes appliquent des règles différentes concernant la durée de validité des mots de passe.

Cette absence d’harmonisation rend les pratiques de sécurité moins cohérentes et complique leur suivi.

**Exploitation possible :**

- Conservation prolongée d’un mot de passe compromis ;
- Utilisation de règles moins strictes sur certains systèmes ;
- Difficulté à appliquer une politique commune.

**Conséquences possibles :**

- Maintien plus long d’un accès compromis ;
- Différences de protection entre les applications ;
- Difficulté à contrôler le respect des règles d’authentification.

### 3.6. Fichiers sensibles non chiffrés sur les terminaux

**Constat :**  
Des fichiers contenant des informations sensibles sont stockés sans chiffrement sur certains terminaux.

**Domaine concerné :**  
Protection des données et sécurité des postes de travail.

**Description :**  
Certaines données sensibles peuvent être directement consultées si une personne accède au terminal ou au support de stockage sur lequel elles sont enregistrées.

Le chiffrement n’est pas systématiquement utilisé pour protéger les données stockées localement.

**Exploitation possible :**

- Accès à un ordinateur perdu ou volé ;
- Consultation directe des fichiers ;
- Copie de données sur un support externe ;
- Extraction d’informations depuis un terminal compromis.

**Conséquences possibles :**

- Divulgation d’informations personnelles ou médicales ;
- Perte de confidentialité ;
- Copie non autorisée de fichiers ;
- Exposition de données en dehors du système d’information.

### 3.7. Réseau Wi-Fi utilisant le protocole WEP

**Constat :**  
Le réseau Wi-Fi utilise encore le protocole WEP.

**Domaine concerné :**  
Sécurité des réseaux sans fil.

**Description :**  
Le protocole WEP utilisé pour protéger le réseau sans fil ne fournit plus un niveau de protection adapté aux exigences actuelles de sécurité.

Les communications et l’accès au réseau peuvent être exposés à des techniques d’interception ou de récupération de clés.

**Exploitation possible :**

- Interception du trafic sans fil ;
- Récupération de la clé de protection ;
- Connexion non autorisée au réseau ;
- Observation des communications.

**Conséquences possibles :**

- Accès à des ressources internes ;
- Interception d’informations ;
- Utilisation du réseau par une personne non autorisée ;
- Facilitation d’autres attaques contre les systèmes internes.

### 3.8. E-mails sensibles transmis sans chiffrement

**Constat :**  
Des e-mails contenant des informations sensibles sont transmis sans chiffrement depuis ou vers des domiciles et des appareils mobiles.

**Domaine concerné :**  
Messagerie et protection des échanges.

**Description :**  
Les informations sensibles peuvent être transmises par courrier électronique sans mécanisme de chiffrement adapté.

Les échanges peuvent également être réalisés depuis des réseaux ou des équipements qui ne sont pas entièrement maîtrisés par l’organisation.

**Exploitation possible :**

- Interception d’un message ;
- Accès à une boîte de messagerie compromise ;
- Consultation d’un message sur un appareil perdu ;
- Envoi d’informations à un destinataire incorrect.

**Conséquences possibles :**

- Divulgation de données sensibles ;
- Perte de confidentialité des échanges ;
- Diffusion d’informations à des personnes non autorisées ;
- Conservation de données sensibles sur des équipements insuffisamment protégés.

### 3.9. Journaux IDS rarement examinés

**Constat :**  
Les journaux du système de détection d’intrusion sont rarement examinés.

**Domaine concerné :**  
Supervision et détection des incidents.

**Description :**  
Les événements enregistrés par le système de détection d’intrusion ne font pas l’objet d’une consultation suffisamment régulière.

Les alertes peuvent donc ne pas être analysées rapidement ou être laissées sans suite.

**Exploitation possible :**

- Maintien d’une activité malveillante non détectée ;
- Répétition d’une tentative d’intrusion ;
- Exploitation prolongée d’une faiblesse ;
- Absence de réaction à une alerte.

**Conséquences possibles :**

- Retard dans la détection d’un incident ;
- Difficulté à reconstituer les événements ;
- Allongement de la durée d’une compromission ;
- Manque d’informations pour l’investigation.

### 3.10. Équipements contenant des données sensibles utilisés à titre privé

**Constat :**  
Certains équipements contenant des données sensibles sont utilisés à des fins personnelles.

**Domaine concerné :**  
Utilisation des équipements et sécurité des terminaux.

**Description :**  
Des équipements professionnels contenant des informations sensibles peuvent être utilisés pour des activités personnelles.

Cette utilisation peut exposer les équipements à des logiciels, des réseaux ou des utilisateurs qui ne relèvent pas du cadre professionnel.

**Exploitation possible :**

- Installation de logiciels non autorisés ;
- Connexion à des réseaux non maîtrisés ;
- Accès par un membre de la famille ou un tiers ;
- Infection du terminal par un logiciel malveillant.

**Conséquences possibles :**

- Accès non autorisé à des données ;
- Compromission du terminal ;
- Copie ou divulgation d’informations ;
- Introduction d’un logiciel malveillant dans l’environnement professionnel.

### 3.11. Postes laissés sans surveillance

**Constat :**  
Des postes de travail sont laissés sans surveillance et les utilisateurs ne se déconnectent pas systématiquement.

**Domaine concerné :**  
Sécurité des postes de travail et contrôle des sessions.

**Description :**  
Des sessions ouvertes restent accessibles lorsqu’un utilisateur quitte temporairement son poste.

Une personne présente dans les locaux peut alors utiliser une session déjà authentifiée.

**Exploitation possible :**

- Consultation d’informations affichées ;
- Utilisation d’une application ouverte ;
- Modification de données ;
- Utilisation de la session d’un autre utilisateur.

**Conséquences possibles :**

- Consultation non autorisée d’informations ;
- Modification de données ;
- Usurpation de session ;
- Difficulté à distinguer l’utilisateur réel de la personne ayant utilisé le poste.

### 3.12. Mises à jour et configurations incohérentes

**Constat :**  
Les mises à jour et les configurations ne sont pas appliquées de manière cohérente.

**Domaine concerné :**  
Administration des systèmes et gestion de la maintenance.

**Description :**  
Les équipements et les systèmes ne disposent pas toujours des mêmes versions, paramètres ou règles de configuration.

Cette situation peut entraîner des différences de protection entre les environnements.

**Exploitation possible :**

- Exploitation d’une version vulnérable ;
- Utilisation d’une configuration insuffisamment sécurisée ;
- Contournement d’un contrôle présent sur un autre système ;
- Exploitation d’une différence entre les environnements.

**Conséquences possibles :**

- Accès non autorisé à certains systèmes ;
- Dysfonctionnements ;
- Difficulté à maintenir un niveau de sécurité homogène ;
- Augmentation de la complexité de l’administration.

### 3.13. Règles de pare-feu trop permissives

**Constat :**  
Les pare-feu autorisent les communications par défaut et bloquent uniquement les flux explicitement refusés.

**Domaine concerné :**  
Contrôle des flux réseau.

**Description :**  
La logique de filtrage utilisée permet potentiellement à des communications de passer lorsqu’elles ne sont pas expressément interdites.

Des services ou des ports qui ne sont pas nécessaires peuvent ainsi rester accessibles.

**Exploitation possible :**

- Connexion à des services non nécessaires ;
- Exploitation de ports ouverts ;
- Communication avec des systèmes internes ;
- Circulation d’un attaquant à l’intérieur du réseau.

**Conséquences possibles :**

- Augmentation des possibilités d’accès au réseau ;
- Facilitation d’une intrusion ;
- Accès à des services internes ;
- Propagation d’une compromission.

### 3.14. Serveurs non corrigés

**Constat :**  
Certains serveurs ne disposent pas des correctifs de sécurité nécessaires.

**Domaine concerné :**  
Maintenance des serveurs et gestion des correctifs.

**Description :**  
Des systèmes serveurs utilisent des versions qui ne sont pas à jour ou qui peuvent contenir des vulnérabilités connues.

L’absence de correctifs laisse certaines faiblesses présentes dans les logiciels ou les systèmes d’exploitation.

**Exploitation possible :**

- Exploitation d’une vulnérabilité connue ;
- Exécution de code malveillant ;
- Élévation de privilèges ;
- Compromission d’un service exposé.

**Conséquences possibles :**

- Accès non autorisé à un serveur ;
- Modification ou extraction de données ;
- Interruption d’un service ;
- Utilisation du serveur comme point d’entrée vers d’autres ressources.

### 3.15. Modification non contrôlée des informations personnelles

**Constat :**  
L’intranet permet à des utilisateurs de modifier des informations personnelles sans contrôle suffisant.

**Domaine concerné :**  
Intégrité des données et contrôle des applications.

**Description :**  
Les mécanismes de contrôle des modifications ne permettent pas toujours de vérifier que l’utilisateur dispose des droits nécessaires pour modifier certaines informations.

Les changements peuvent également ne pas être suffisamment validés ou tracés.

**Exploitation possible :**

- Modification d’informations par un utilisateur non autorisé ;
- Utilisation d’un compte compromis ;
- Modification accidentelle de données ;
- Altération volontaire d’informations personnelles.

**Conséquences possibles :**

- Perte d’intégrité des données ;
- Erreurs dans les informations enregistrées ;
- Difficulté à identifier l’auteur d’une modification ;
- Utilisation de données incorrectes dans les activités de l’organisation.

## 4. Synthèse des domaines concernés

Les 15 vulnérabilités identifiées concernent plusieurs domaines de la sécurité des systèmes d’information.

| Domaine | Vulnérabilités concernées |
|---|---|
| Gestion des accès et des habilitations | Comptes d’anciens employés, privilèges excessifs |
| Authentification | Mots de passe facilement déchiffrables, expiration non standardisée |
| Accès distant | Accès à distance non sécurisé |
| Protection des données | Fichiers non chiffrés, e-mails sans chiffrement |
| Sécurité réseau | Wi-Fi WEP, règles de pare-feu trop permissives |
| Supervision | Journaux IDS rarement examinés |
| Sécurité des terminaux | Utilisation privée d’équipements sensibles, postes sans surveillance |
| Administration des systèmes | Mises à jour et configurations incohérentes, serveurs non corrigés |
| Intégrité des données | Modification non contrôlée des informations personnelles |

## 5. Conclusion

L’analyse des vulnérabilités montre que les faiblesses d’ACME Healthcare touchent à la fois les aspects techniques, organisationnels et humains de la sécurité.

Les constats concernent notamment :

- La gestion des comptes et des droits ;
- La protection des authentifications ;
- La sécurisation des accès à distance ;
- La protection des données stockées et échangées ;
- La configuration des réseaux ;
- La supervision des événements ;
- La maintenance des systèmes ;
- Le contrôle des modifications de données.

Cette analyse permet de disposer d’une vision structurée des faiblesses identifiées.

La partie suivante consistera à évaluer les risques associés à ces vulnérabilités et à déterminer les constats qui doivent être traités en priorité.
