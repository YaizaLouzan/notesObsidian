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

