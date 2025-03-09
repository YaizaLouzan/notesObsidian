# Services cloud

## IaaS
-> Infrastructure As A Service

C'est un modèle où les utilisateurs louent des ressources informatiques telles que des serveurs, du stockage et des réseaux via internet, leur permettant de gérer entièrement leur infrastructure sans avoir à investir dans du matériel physique. Exemples : **Amazon EC2, Microsoft Azure Virtual Machines**.

Exemple : VM

## PaaS
-> Platform As A Service

Ce modèle fournit une plateforme complète permettant aux développeurs de créer, déployer et gérer des applications sans se soucier de l'infrastructure sous-jacente. Cela inclut des outils de développement, des bases de données et des services middleware. Exemples : **Google App Engine, Microsoft Azure App Service**.

Exemple : Application que l'on développe

## SaaS
-> **Software as a Service**

C'est un modèle où les utilisateurs accèdent à des applications via internet sans avoir besoin de les installer ou de les gérer localement. Les mises à jour et la maintenance sont gérées par le fournisseur. Exemples : **Google Workspace, Microsoft 365**.

Exemple : Site web

## FaaS
**-> Function as a Service**

Ce modèle permet aux utilisateurs d'exécuter des fonctions ou des morceaux de code en réponse à des événements, sans gérer l'infrastructure. C'est souvent utilisé pour des applications basées sur des microservices. Exemples : **AWS Lambda, Azure Functions**.

## Modèle de responsabilité partagée
Le **modèle de responsabilité partagée** dans les services cloud définit la répartition des responsabilités entre le fournisseur de services cloud et le client en matière de sécurité et de gestion des ressources. Voici comment cela fonctionne pour chaque modèle de service :

1. **IaaS (Infrastructure as a Service)** :
    
    - **Responsabilité du fournisseur** : Fournir l'infrastructure physique, la sécurité des datacenters, et les composants réseau.
    - **Responsabilité du client** : Gérer le système d'exploitation, les applications, les données et la sécurité au niveau de la configuration.
2. **PaaS (Platform as a Service)** :
    
    - **Responsabilité du fournisseur** : Gérer l'infrastructure sous-jacente, la plateforme, et les mises à jour logicielles.
    - **Responsabilité du client** : Développer, gérer et sécuriser les applications qu'il déploie sur la plateforme.
3. **SaaS (Software as a Service)** :
    
    - **Responsabilité du fournisseur** : Gérer l'application, l'infrastructure sous-jacente, la sécurité des données, et les mises à jour.
    - **Responsabilité du client** : Gérer les utilisateurs, les permissions, et la configuration de l'application selon ses besoins.
4. **FaaS (Function as a Service)** :
    
    - **Responsabilité du fournisseur** : Gérer l'infrastructure et le runtime pour exécuter les fonctions.
    - **Responsabilité du client** : Écrire et gérer le code des fonctions, ainsi que la logique de sécurité des données traitées.

En résumé, plus tu descends dans la pile des modèles (d'IaaS à SaaS), plus la responsabilité du fournisseur augmente, tandis que celle du client diminue.

# Modèles cloud

![[Pasted image 20250309151606.png]]

## Cloud privé
Environnement dédié à une seule organisation, hébergé sur site ou par un tiers. **Accès limité et contrôle accru sur la sécurité des données.** 
Exemples : 
- VMWare Cloud 
- OpenStack

✅ **Avantages** :

- Sécurité et confidentialité accrues (environnement dédié).
- Personnalisation possible selon les besoins spécifiques.
- Peut être hébergé chez un fournisseur ou sur site.

❌ **Inconvénients** :

- Coût élevé (matériel, maintenance, experts IT).
- Moins flexible que le cloud public en cas de pics de demande.
- Mise en place plus complexe.
## Cloud public
Fournit des ressources partagées (serveurs, stockage) via un fournisseur tiers. **Accès à travers Internet, ressources partagées entre plusieurs clients.**
Exemples : 
- AWS
- Microsoft Azure
- Google Cloud

✅ **Avantages** :

- Coût réduit (pas besoin d’acheter du matériel).
- Évolutivité rapide (ajout de ressources à la demande).
- Maintenance et mises à jour gérées par le fournisseur.
- Accessibilité mondiale et haute disponibilité.

❌ **Inconvénients** :

- Moins de contrôle sur la sécurité et la gestion des données.
- Dépendance au fournisseur (risque de "lock-in").
- Peut être coûteux à long terme pour des usages intensifs.
## Cloud hybride
Combine cloud public et privé, offrant flexibilité et scalabilité. **Permet d'utiliser des ressources internes et externes selon les besoins.**
Exemples : 
- Applications critiques sur cloud privé
- Scalabilité via cloud public.

✅ **Avantages** :

- Équilibre entre flexibilité et sécurité.
- Possibilité de garder des données sensibles en privé et le reste en public.
- Optimisation des coûts en combinant les deux modèles.

❌ **Inconvénients** :

- Complexité de gestion et d’intégration.
- Nécessite une bonne coordination entre les différents environnements.
# Cloud on-permise
C'est une infrastructure hébergée et gérée **localement** dans les locaux de l'entreprise. Elle **adopte des principes du cloud** (virtualisation, automatisation, gestion des ressources) et offre un **contrôle total sur les données** et systèmes, tout en permettant certains avantages du cloud, tels que l'élasticité et l'optimisation des ressources. Convient aux organisations ayant des exigences strictes en matière de sécurité et de conformité.

✅ **Avantages** :

- Contrôle total sur les infrastructures et la sécurité.
- Performances optimisées selon les besoins internes.
- Pas de dépendance à un fournisseur externe.

❌ **Inconvénients** :

- Coût très élevé (achat, maintenance, énergie).
- Besoin d’une équipe IT compétente.
- Moins flexible pour faire évoluer rapidement les ressources.

**Résumé rapide** :

- **On-Premise** = Serveurs **chez vous**, gestion 100% interne.
- **Cloud Privé** = Serveurs **dédiés pour vous**, mais hébergés ailleurs et/ou gérés par un prestataire.

# Modèle de consommation
Les fournisseurs de services cloud (ex. AWS, Microsoft Azure) fonctionnent principalement avec le modèle OpEx, permettant aux utilisateurs de payer uniquement pour les ressources qu'ils consomment, sans frais initiaux ni gestion complexe d'infrastructure.