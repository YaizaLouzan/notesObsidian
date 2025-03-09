- identité et ce machin

	- entra id
	- azure a dds
	- auth

		- MFA et SSO et machin (petite définition)

	- acces conditionnel

- diff entre auth et autorisation (authz et auth?)
- azure MFA
- b2b , b2c expliquer simplement
- accès conditionnel - important

	- a quoi ca peut servir

- RBAC azure
- zero thrust
- défense en profondeur
- microsoft defender

# Locataire Azure
Un **locataire Azure** est une **instance dédiée et approuvée d'Azure Active Directory (Azure AD)**, automatiquement créée lorsque votre organisation souscrit à un service cloud Microsoft. Ce locataire représente une seule organisation et sert de base pour la gestion des identités et des accès dans un environnement cloud sécurisé.

Contient:
- Annuaire Azure AD dédié
- Gestion des identités et des accès
- **Isolations des ressources**
	- Le locataire Azure est isolé
- Création automatique

**le terme Tenant désigne la bulle (le nuage) dans laquelle vos données vont être stockées**.

# Microsoft Entra ID

-> Comme un AD ! C'est l'Active directory de Azure.

Fonctionnalités:

- **Authentification des employés**
	- Les utilisateurs peuvent se connecter en toute sécurité pour accéder à des ressources critiques, qu'elles soient locales ou dans le cloud.
- **Authentification unique (SSO)**
	- Permet aux utilisateurs de se connecter une seule fois pour accéder à toutes les applications et services autorisés, sans avoir à se reconnecter pour chaque application.
- **Gestion des applications**
	- permet aux entreprises de centraliser et de contrôler l'accès aux applications utilisées par leurs employés
## Services B2B (Business to business)
Fonctionnalité utilisée lorsque vous voulez collaborer avec **des membres d'autres organisations**

### Principes
1. Inviter des utilisateurs externes  
2. Pas besoin de créer des comptes dans votre annuaire
    - Les utilisateurs gardent leurs identités d'origine (leurs propres identifiants). Cela réduit la gestion des identités dans votre système.
3. Sécurité renforcée
    - Vous pouvez appliquer vos **politiques de sécurité** 

## Services B2C (business to Customer)
**Pour gérer des utilisateurs externes finaux (vos clients)** 
Azure AD B2C est conçu pour les **entreprises** qui interagissent avec des clients ou utilisateurs finaux. Ces derniers se connectent à vos **applications grand public**.

### Principes
1. **Créer une expérience utilisateur personnalisée** :
    - Azure AD B2C vous permet de créer des pages de connexion/inscription **avec votre marque** (logo, design, etc.). Vos clients peuvent s'inscrire et se connecter à vos applications.    
2. **Gérer les identités des clients** :
    - Vos clients peuvent utiliser **leur propre compte** (par ex. Google, Facebook, Microsoft) ou créer un nouveau compte avec une adresse e-mail et un mot de passe.  
3. **Haute sécurité pour les applications grand public** :
    - Authentification multi-facteurs et autres mesures pour protéger les comptes de vos clients.    
4. **Évolutivité** :
    - Conçu pour gérer des millions de clients finaux.

# Azure Active Directory Domain Services

-> l'AD DS de Azure

Azure AD DS fournit des fonctionnalités AD dans le cloud, sans nécessiter de gestion de controleurs de domaine.

Avantages:

- Gestion simplifiée
- Compatibilité
- Sécurité intégrée
# Accès conditionnel
Les contrôles d'accès conditionnel dans Azure permettent de sécuriser l'accès aux ressources en appliquant des conditions spécifiques, assurant ainsi une protection adaptée tout en offrant une expérience utilisateur fluide.

## Principales Conditions

1. **Emplacement :** Restriction d'accès selon la géolocalisation de l'utilisateur.
2. **Appareil :** Vérification de la conformité de l'appareil aux politiques de sécurité.
3. **Application :** Application de conditions spécifiques pour chaque application.
4. **Utilisateurs et Groupes :** Application de politiques selon les groupes d'utilisateurs ou les rôles.

## Actions 

- **Accorder l'accès :** Permet l'accès si les conditions sont remplies.
- **Bloquer l'accès :** Refuse l'accès si les conditions ne sont pas satisfaites.
- **Exiger une authentification supplémentaire :** Par exemple, une authentification multi-facteurs pour renforcer la sécurité.
# Authentification
## Azure Multi-Factor Authentification

Azure MFA est une méthode de sécurité renforcée qui exige au moins deux éléments d'authentification avant d'accorder un accès.

### Trois catégories de facteurs utilisées dans la MFA

- Quelque chose que vous connaissez :

Il s'agit généralement d'un **mot de passe, d'un code PIN, ou d'une réponse à une question de sécurité**. Ce facteur est la première ligne de défense, mais peut être vulnérable en cas de vol ou de piratage.

- Quelque chose que vous possédez :

Cela inclut des **objets physiques ou numériques que vous avez en votre possession**, comme un **smartphone qui reçoit une notification** via une application mobile (ex : Microsoft Authenticator), ou un appareil générateur de jetons (comme un token physique ou une clé de sécurité).

Ce facteur ajoute une barrière supplémentaire en s'assurant que seul l'utilisateur ayant l'objet ou l'appareil peut se connecter.

- Quelque chose que vous êtes :

Ce facteur fait référence à une c**aractéristique biométrique unique à l'utilisateur**, telle qu'une **empreinte digitale, un scan du visage ou de l'iris**. De nombreux appareils mobiles modernes intègrent cette technologie pour une authentification plus rapide et sécurisée.

## Comparaison entre authentification et autorisation
- **Authentification** : s'assurer de **qui vous êtes**.
- **Autorisation** : déterminer **ce que vous êtes autorisé à faire**.
### Authentification - AuthN
- Identifie la personne ou le service cherchant à accéder à une ressource
- Demande des informations d’identification d’accès légitimes
- Sert de fondement pour créer des principes sécurisés d’identité et de contrôle d’accès

### Autorisation - AuthZ
- Détermine le niveau d’accès d’une personne authentifiée ou d’un service
- Définit les données auxquelles ils peuvent accéder et ce qu’ils peuvent en faire