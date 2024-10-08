## Stratégie de sécurisation

### **Introduction générale**
- **Défense en profondeur**
    - *Pourquoi le mettre en place ?*
    - *Pour lutter contre quoi ? Dans quel contexte ?*
- **Réduction de la surface d'attaque**
    - *Pourquoi le mettre en place ?*
    - *Pour lutter contre quoi ? Dans quel contexte ?*
- **RGPD (Règlement Général sur la Protection des Données)**:
  <!-- - *Données personnelles* 
  - *Données sensibles* 
  - *Données critiques*  -->
    - *Pourquoi le mettre en place ?*
    - *Pour lutter contre quoi ? Dans quel contexte ?*
    - *Consentement et conformité avec la réglementation en vigueur*

### **Back-end**

#### Introduction
1. Politique de moindre privilège
- *Pourquoi ?*
- *Pour lutter contre quoi ? Dans quel contexte ?*
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
      - Automatisation
        - *Nombre*
        - *Fréquence*
    - Politique de rétention
        - Nombre de sauvegardes
        - Support (stockage)


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

#### Protocoles de sécurité (côté front-end)
- HTTP + TLS = HTTPS
    - HSTS
    - TLS
- SOP
- CSP
  - Referrer Policy
  - SRI