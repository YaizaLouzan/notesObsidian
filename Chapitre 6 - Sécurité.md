# Locataire Azure

Contient:

- Annuaire Azure AD dédié
- Gestion des identités et des accès
- Isolations des ressources
- Création automatique

# Microsoft Entra ID

-> Comme un AD ! C'est l'Active directory de Azure.

Fonctionnalités:

- Authentification des employés
- Authentification unique (SSO)
- Gestion des applications
- Services B2B (Buissiness to buissiness)
- Services B2C (buissiness to customer)

Azure Active Directory Domain Services

-> l'AD DS de Azure

Azure AD DS fournit des fonctionnalités AD dans le cloud, sans nécessiter de gestion de controleurs de domaine.

Avantages:

- Gestion simplifiée
- Compatibilité
- Sécurité intégrée

Azure Multi-Factor Authentification

Méthode de sécurité renforcée qui exige au moins deux éléments d'authentification avant d'accorder un accès.

TROIS CATEGORIES DE FACTEURS UTILISES DANS LA MFA

- Quelque chose que vous connaissez :

Il s'agit généralement d'un mot de passe, d'un code PIN, ou d'une réponse à une question de sécurité. Ce facteur est la première ligne de défense, mais peut être vulnérable en cas de vol ou de piratage.

- Quelque chose que vous possédez :

Cela inclut des objets physiques ou numériques que vous avez en votre possession, comme un smartphone qui reçoit une notification via une application mobile (ex : Microsoft Authenticator), ou un appareil générateur de jetons (comme un token physique ou une clé de sécurité).

Ce facteur ajoute une barrière supplémentaire en s'assurant que seul l'utilisateur ayant l'objet ou l'appareil peut se connecter.

- Quelque chose que vous êtes :

Ce facteur fait référence à une caractéristique biométrique unique à l'utilisateur, telle qu'une empreinte digitale, un scan du visage ou de l'iris. De nombreux appareils mobiles modernes intègrent cette technologie pour une authentification plus rapide et sécurisée.

External Identities - accès et sécurité azure

MODELE B2B

- pour collaborer avec des partenaires externes
- avantages

- accès sécurisé: partenaires se connectent avec leurs propres identifiants sans créer un compte externe
- contrôle acces granulaire: chaque partenaire despose des droits nécessaires, sans compromis sur la sécurité.

MODELE B2C

- permets aux entreprises de gérer l'authentification et id de leurs clients
- permet de se connecter à des applications web ou mobiles via leurs identifiants de réseaux sociaux ou en créant u compte personnel
- avantages:

- meilleire experience utilisateur: les cliens peuvent choisir leur méthode de connexion préférée
- gestion sécurisée des identités client: assure la sécurité et la confidentialité des informations client

Accès conditionnel

Les contrôles d'accès conditionnel dans Azure permettent de sécuriser l'accès aux ressources en appliquant des conditions spécifiques, assurant ainsi une protection adaptée tout en offrant une expérience utilisateur fluide.

Conditions:

- Emplacement: restriction d'accès selon la géolocalication de l'user
- appareil: vérification de la conformité de l'appareil aux politiques de sécurité
- application: application de conditions spécifiques pour chaque application
- utilisateurs et groupes: application de politiques selon les groupes d'user ou les rôles

Actions:

- accorder l'accès si conditions remplies
- bloquer l'accès si conditions non remplies
- exiger une authentification supplémentaire pour renforcer la sécurité

Contrôle d'accès en fonction du rôle Azure (Azure RBAC)

RBAC : Role Based Access Control

Permet de gérer les accès aux ressources azure en fonction de rôles spécifiques. Les rôles peuvent être assignés à différents niveaux (abonnement, groupe de ressources, ressource spécifique)

RÔLES PRINCIPAUX :

- Lecteur: peut uniquement voir les ressources
- contributeur: peut modifier les ressources sans gérer les accès
- propriétaire: peut modifier les ressources et gérer les accès

ATTRIBUTION DES RÔLES :

Une fois que vous avez les rôles, vous devez les assigner aux personnes ou groupes qui en ont besoin. Vous pouvez attribuer ces rôles à différents niveaux :

- Au niveau de l'abonnement : Cela donne accès à toutes les ressources sous un abonnement spécifique.
- Au niveau du groupe de ressources : Cela donne accès uniquement aux ressources dans un groupe de ressources particulier.
- Au niveau de la ressource : Cela donne accès à une ressource spécifique, comme une machine virtuelle ou un compte de stockage.

AVANTAGES:

- gestion simplifiée
- sécuritée renforcée
- flexibilité

Confiance zéro

Approche de sécurité qui suppose que les menaces peuvent exister à l'intérieur du réseau ainsi qu'à l'extérieur. Au lieu de faire confiance automatiquement à quelqu'un parce qu'il se trouve à l'intérieur du périmètre sécurisé de l'entreprise, cette approche vérifie systématiquement chaque demande d'accès, peu importe d'où elle provient.

Comment ça fonctionne ?

- Vérifier explicitement

- Chaque demande d'accès est systématiquement authentifiée et autorisée en fonction de tous les points de données disponibles. Cela signifie que le système évalue de manière continue et complète la légitimité de chaque utilisateur, appareil et application qui tente d'accéder aux ressources.

- Utiliser l'accès avec le privilège minimum

- La Confiance Zéro privilégie le principe du moindre privilège, ce qui signifie que les utilisateurs n'ont accès qu’aux ressources nécessaires pour accomplir leurs tâches. On utilise souvent l’accès juste-à-temps (JIT) et juste suffisant (JEA) pour limiter les droits d’accès de manière temporaire et précise. Les stratégies adaptatives permettent d'ajuster les permissions en fonction des besoins actuels et du contexte.

- envisager les violations de sécurité

- En cas de compromission, il est crucial de réduire le rayon d’explosion. Cela se fait en segmentant le réseau en zones plus petites pour limiter les déplacements latéraux des attaquants. De plus, le chiffrement de bout en bout est vérifié pour protéger les données en transit et garantir leur sécurité tout au long de leur parcours.

Défense en profondeur

approche de sécurité qui utilise plusieurs couches de protection pour réduire les risques. Chaque couche de sécurité joue un rôle spécifique, et l'idée est que même si un attaquant parvient à contourner une couche, d’autres couches de défense continueront de protéger les systèmes.

Les Couches de la Défense en Profondeur :

1. Sécurité Physique (Physical Security) : La première ligne de défense protège le matériel informatique dans les centres de données. Cela inclut les contrôles d'accès physiques comme des serrures, des cartes d'accès, et des caméras de surveillance pour s'assurer que seuls les employés autorisés peuvent entrer dans les zones sensibles où sont stockés les serveurs et les équipements.
2. Identités et Accès (Identity and Access Management) : Cette couche contrôle qui peut accéder à l'infrastructure et apporter des modifications. On utilise des méthodes telles que l'authentification multi-facteurs (MFA) pour vérifier l'identité des utilisateurs et gérer les permissions afin de garantir que seules les personnes autorisées peuvent accéder aux systèmes et aux données.
3. Périmètre (Perimeter Security) : Cette couche protège contre les attaques à grande échelle, comme les attaques par déni de service distribué (DDoS). On déploie des systèmes de filtrage pour empêcher les attaques massives de surcharger les services et les rendre inaccessibles aux utilisateurs, ce qui aide à maintenir la disponibilité et la performance des services.
4. Réseau (Network Security) : Cette couche limite les communications entre les différentes ressources au sein du réseau. On utilise des techniques de segmentation du réseau et des contrôles d'accès pour s'assurer que les ressources critiques sont isolées et protégées, réduisant ainsi les risques de propagation d'une attaque à d'autres parties du réseau.
5. Calcul (Compute Security) : Cette couche protège l'accès aux machines virtuelles et autres environnements de calcul. On met en place des contrôles pour sécuriser les machines virtuelles, notamment par des configurations sécurisées et une gestion appropriée des accès pour empêcher les modifications non autorisées.
6. Application (Application Security) : Cette couche assure que les applications sont sécurisées et exemptes de vulnérabilités. On intègre des pratiques de sécurité tout au long du développement des applications pour identifier et corriger les failles de sécurité, y compris des tests de sécurité réguliers et des mises à jour pour protéger les applications contre les menaces.
7. Données (Data Security) : Cette couche contrôle l'accès aux données commerciales et clients sensibles. On met en œuvre des mécanismes de chiffrement pour protéger les données lorsqu'elles sont stockées ou transmises, ainsi que des contrôles d'accès rigoureux pour garantir que seules les personnes autorisées peuvent consulter ou modifier les informations sensibles.

Microsoft Defender pour le cloud

service de sécurité qui offre une protection complète pour vos ressources cloud et locaux (services hybrides). Il surveille en permanence vos systèmes et vous alerte en cas de menaces potentielles. Il aide également à renforcer votre sécurité en vous fournissant des recommandations et des outils pour corriger les vulnérabilités.

- Suggestions en matière de sécurité
- Détection et blocage des programmes malveillants
- Analyse et identification des attaques potentielles
- Contrôle des accès en flux tendus pour les ports
- Intégré en mode natif dans Azure