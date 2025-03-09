Capacité de traiter des données et d'exécuter des applications

- Serverless
Le développeur ne gère que le code de l’application, le fournisseur provisionne, dimensionne et gère les serveurs sans intervention manuelle.

Vous n'avez pas à vous soucier des serveurs, des machines ou de la gestion des ressources, tout est automatisé

exécute une fonction quand on le demande. on sera facturé par rapport au nbre de fois qu'n l'exécute

- Bare Metal
Serveurs physiques dédiés, offrant des performances maximales tout en bénéficiant de la flexibilité du cloud. **Exemples** : AWS Bare Metal Instances, IBM Cloud Bare Metal Servers

- Conteneurs
Des unités légères qui encapsulent les applications et leurs dépendances pour un déploiement rapide et une grande portabilité.

Exemples : Amazon ECS, Google Kubernetes Engine.

- Machines Virtuelles
Exemples : Amazon EC2, Microsoft Azure VMs, Google Compute Engine.


| Option de calcul                             | Modèle de cloud                    |
| -------------------------------------------- | ---------------------------------- |
| 🖥 **Machines Virtuelles (VMs)**             | IaaS (Infrastructure as a Service) |
| 📦 **Conteneurs (Docker, Kubernetes, etc.)** | IaaS / PaaS                        |
| 🔧 **Bare Metal**                            | IaaS                               |
| Serverless                                   | Faas / PaaS                        |

# Services de calcul réseau Azure
Communication sécurisée entre les ressources Azure, Internet, et les réseaux locaux.

- **Points de terminaison publics** : accessibles depuis n'importe où sur Internet.
- **Points de terminaison privés** : accessibles uniquement depuis votre réseau interne.
- **Sous-réseaux virtuels**: segmentation de votre réseau selon vos besoins.
- **Appairage de réseaux** : connectez directement vos réseaux privés ensemble pour une meilleure intégration.

## Azure Virtual Desktop
Service de virtualisation de bureau et d’application, permet de créer un environnement complet de virtualisation de bureau

## Azure Containers Services

Les conteneurs Azure offrent un environnement virtualisé léger ne nécessitant pas de gérer le système d’exploitation mais capable de répondre aux changements à la demande

## Azure Fonctions : serverless
C'est une solution serverless qui permet d'écrire moins de code, maintenir moins d'infrastructure et moins coûteuse.
Serverless rapproche les développeurs de la logique métier tout en les isolant des problèmes d’infrastructure. Il s’agit d’un modèle qui n’implique pas « aucun serveur », mais plutôt « moins de serveurs »

# Services de mise en réseau Azure
## Le réseau virtuel Azure (VNet)

Le réseau virtuel Azure (VNet) permet aux ressources Azure de communiquer en toute sécurité entre elles, sur Internet et sur les réseaux locaux.

On distingue:

- Points de terminaison publics, accessibles depuis n’importe où sur Internet
- Points de terminaison privés, accessibles seulement depuis votre réseau
- Sous-réseaux virtuels : permettant de segmenter votre réseau en fonction de vos besoins
- Appairage de réseaux : connectez vos réseaux privés directement ensemble.

## Passerelle de réseau privé virtuel (VPN)

Le VPN d'Azure est un service qui permet de créer une **connexion sécurisée** entre le réseau local d'une entreprise (comme celui de ses bureaux ou son centre de données) et le **cloud Azure**, en utilisant **Internet**. Contrairement à **ExpressRoute**, qui utilise une connexion privée, le VPN d'Azure passe par une connexion publique, mais il chiffre les données pour garantir la **sécurité**.

Azure propose deux types de connexions VPN :

- **Site à site** : Ce type de VPN connecte **deux réseaux différents** (le réseau local d'une entreprise et le cloud Azure) via un tunnel VPN sécurisé. Il est généralement utilisé pour connecter des bureaux distants au cloud.
    
- **Point à site** : Ce type de VPN permet aux **utilisateurs individuels** (comme les employés travaillant à distance) de se connecter au cloud Azure depuis leur **ordinateur personnel** ou un autre appareil. Ils peuvent ainsi accéder aux ressources de l'entreprise de manière sécurisée depuis n'importe où.
    

**Avantages:**

- **Sécurité** 
- **Flexibilité** 
- **Coût** 
- **Simplicité**

## Azure ExpressRoute
Service de Microsoft Azure qui permet de **créer une connexion directe entre le réseau local d'une entreprise et le cloud Azure, sans passer par Internet**. En général, Azure ExpressRoute fonctionne en collaboration avec des **fournisseurs de services** locaux, qui mettent en place une connexion privée (souvent via la fibre optique ou des réseaux privés) entre le réseau de l’entreprise et le cloud d’Azure. Cela permet d'établir un **accès dédié** aux ressources d'Azure, sans transiter par Internet.

- **Performance optimisée** : ExpressRoute évite les embouteillages d’Internet en offrant une connexion rapide avec une **latence faible**, idéale pour les applications critiques qui nécessitent une réactivité immédiate.
    
- **Sécurité renforcée** : La connexion ne transite pas par Internet, ce qui réduit considérablement les risques d’interceptions ou de **cyberattaques**.
    
- **Fiabilité accrue** : ExpressRoute est conçu pour être plus stable et offrir une meilleure **continuité de service**, ce qui est essentiel pour les entreprises qui dépendent de services cloud pour leurs opérations.

## Azure DNS service

Azure DNS est conçu pour être **rapide** et **fiable** grâce à un réseau mondial de serveurs DNS répartis dans plusieurs centres de données. Il utilise une technologie appelée **Anycast**, qui permet d’envoyer les requêtes DNS (celles qui convertissent les noms de domaine en adresses IP) vers le **serveur le plus proche** de l’utilisateur. Cela garantit que les **temps de réponse** sont plus rapides, peu importe où se trouve l’utilisateur dans le monde, et cela améliore également la **disponibilité** du service.

Azure DNS tire parti de la sécurité offerte par **Azure Resource Manager**, qui est la plateforme de gestion des ressources dans Azure. Un aspect clé de cette sécurité est le **RBAC** (**Role-Based Access Control**).

En plus de cela, Azure DNS propose :

- **La journalisation** : Toutes les actions et modifications effectuées sur les ressources DNS sont enregistrées, ce qui permet de suivre ce qui a été fait et par qui.
    
- **Le verrouillage des ressources** : Cela empêche les modifications accidentelles ou non autorisées sur les zones DNS.
    

Azure DNS permet de gérer aussi bien des ressources DNS pour des services Azure que pour des **services externes** (par exemple, des domaines que vous possèdez, mais qui ne sont pas hébergés sur Azure). Cela signifie que vous pouvez centraliser la gestion de **tous vos domaines** en utilisant un seul outil, ce qui facilite grandement l’administration de tes noms de domaine.

Avec Azure DNS, il est possible de créer des **noms de domaine privés** personnalisés dans les **réseaux virtuels** d’une entreprise (appelés **VNet** dans Azure). Cela permet aux entreprises de gérer leurs propres services internes avec des **noms de domaine sur mesure**, qui ne sont pas visibles depuis Internet. C’est utile pour des entreprises qui veulent isoler certains services pour des raisons de sécurité ou d’organisation interne.
### RBAC 
Le **contrôle d'accès basé sur les rôles (RBAC)** est un système qui permet de **limiter l’accès** aux ressources en fonction des rôles des utilisateurs. Autrement dit, chaque personne dans une entreprise a des **droits** spécifiques en fonction de son **rôle** :

- Par exemple, un administrateur système peut avoir accès à tout, tandis qu’un développeur pourrait seulement avoir accès à certaines zones DNS.
    
- RBAC garantit que **seules les personnes autorisées** peuvent modifier ou consulter certaines ressources, ce qui renforce la **sécurité** et empêche les erreurs ou les changements accidentels.
### Anycast
**Anycast** est une technique de routage utilisée dans les réseaux informatiques, qui permet d'envoyer une requête à plusieurs serveurs en même temps, mais en assurant que la réponse vienne du **serveur le plus proche** ou le plus accessible.

Dans un système **Anycast**, plusieurs serveurs partagent une même adresse IP publique. Lorsqu'une requête est envoyée à cette adresse, le réseau choisit automatiquement **le serveur le plus proche** en fonction de la position géographique ou des conditions du réseau, comme la latence ou la congestion ou la disponibilité.