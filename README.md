## Stratégie de sécurisation

### **Introduction générale**
- **Défense en profondeur** : Approche de sécurité multicouche pour protéger les systèmes contre les menaces.
- **Réduction de la surface d'attaque** : Minimiser les points d'entrée potentiels pour les attaques.
- **RGPD (Règlement Général sur la Protection des Données)** :
  - **Données personnelles** : Informations identifiables concernant un individu.
  - **Données sensibles** : Informations nécessitant une protection accrue.
  - **Données critiques** : Informations essentielles pour le fonctionnement de l'organisation.
  - **Consentement et conformité** : Demander le consentement des clients, offrir des droits de rectification, et assurer la conformité avec la réglementation en vigueur.
- **Journalisation** : Enregistrement des actions et événements pour l'analyse et la détection des incidents.

### **Back-end**

#### Introduction
1. **Politique de moindre privilège** : Limiter les accès aux ressources au strict nécessaire.
2. **RBAC (Role-Based Access Control)** : Contrôle d'accès basé sur les rôles pour gérer les autorisations.

#### Base de Données (BDD)

- **Politique des mots de passe** :
  - **Hachage** : Transformation des mots de passe en une chaîne sécurisée.
  - **Salage** : Ajout d'une valeur aléatoire aux mots de passe avant le hachage pour renforcer la sécurité.
  
- **Utilisation des UUID** : Utilisation d'identifiants uniques universels pour éviter les collisions et renforcer la sécurité.

- **Politique de rétention (sauvegarde)** : Stratégies pour conserver et sauvegarder les données de manière sécurisée.

#### API

- **Sécurisation des communications** :
  - **TLS (Transport Layer Security)** : Protocole pour sécuriser les communications sur Internet.

- **Sécurité des origines** :
  - **SOP (Same-Origin Policy)** : Politique de sécurité limitant l'interaction entre ressources de différentes origines.
  - **CORS (Cross-Origin Resource Sharing)** : Mécanisme permettant le partage de ressources entre différentes origines.
  - **CSP (Content Security Policy)** *(R13 -> R20)* : Politique utilisée pour contrôler quelles ressources peuvent être chargées par une page web.

- **Utilisation d'un ORM (Object-Relational Mapping)** : Outil pour interagir avec la base de données en utilisant des objets.

- **Authentification** :
  - **Token** : Utilisation de jetons pour gérer l'authentification et les sessions utilisateur.

### **Front-end**

#### Introduction
- **Jamais faire confiance au client (navigateur) -> règle d'or** :
  - Le client, c'est-à-dire le navigateur, ne doit jamais être considéré comme sécurisé. Les actions malveillantes peuvent être tentées intentionnellement ou à travers des scripts non sécurisés.

#### Différents types d'attaque
- **Injection SQL** : Technique d'injection permettant d'exécuter des requêtes SQL malveillantes.
- **Cross-Site Scripting (XSS)** : Injection de scripts malveillants dans une page web vue par d'autres utilisateurs.
- **Cross-Site Request Forgery (CSRF)** : Exploitation qui force un utilisateur authentifié à exécuter des actions non désirées.
- **Clickjacking** : Technique trompant un utilisateur à cliquer sur quelque chose différent de ce qu'il perçoit.
- **Injections de dépendances** : Attaques visant à compromettre les bibliothèques ou modules utilisés par une application.
- **Attaques par force brute (bruteforce)** : Tentatives répétées pour deviner un mot de passe ou une clé cryptographique.
- **Attaques par déni de service (DoS)** et par déni de service distribué (DDoS) : Attaques visant à rendre un service indisponible en surchargeant le système.