## Stratégie de sécurisation

### **Introduction générale**
- **Défense en profondeur**
    - *Pourquoi le mettre en place ?*
    - *Comment ?*
- **Réduction de la surface d'attaque**
    - *Pourquoi le mettre en place ?*
    - *Comment ?*
- **RGPD (Règlement Général sur la Protection des Données)**:
  <!-- - *Données personnelles* 
  - *Données sensibles* 
  - *Données critiques*  -->
    - *Pourquoi le mettre en place ?*
    - *Comment ?*
    - *Consentement et conformité avec la réglementation en vigueur*

### **Back-end**

#### Introduction
1. Politique de moindre privilège
- *Pourquoi ?*
- *Comment ?*
2. RBAC (Role-Based Access Control)

#### Base de Données (BDD)

- **Politique des mots de passe** :
  - *Hachage*
  - *Salage* 
  - *Complexité*
    - *Longueur minimale*
    - *Robustesse*
- Utilisation des UUID
- Politique de rétention :
    - Sauvegarde   
        - *Nombre*
        - *Fréquence*
        - *Heure*


#### API

- *Sécurisation des communications* :
  - TLS (Transport Layer Security)
  - HSTS

- **Sécurité des origines** :
  - *SOP (Same-Origin Policy) : même origine*
    - *CORS (Cross-Origin Resource Sharing) : différentes origines*
  - *CSP (Content Security Policy) : différentes ressources*
- *Utilisation d'un ORM (Object-Relational Mapping)*
- **Authentification** :
  - *Token*
- *Limitation d'appel API*

### *Front-end*

#### Introduction
- *Jamais faire confiance au client (navigateur) -> règle d'or* 

#### Différents types d'attaque
- *Injection SQL*
- *Cross-Site Scripting (XSS)* 
- *Cross-Site Request Forgery (CSRF)* 
- *Clickjacking* 
- *Injections de dépendances*
- *Attaques par force brute (bruteforce)*
- *Attaques par déni de service (DoS)* 

#### Sécurisation

- **Sécurisation des communications** :
  - *HTTPS*
<br>
