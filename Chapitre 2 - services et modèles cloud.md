- services et modèles cloud

- modèles de cloud

- IaaS (ex: VM) , PaaS (ex: Application uq'on développe), SaaS (ex: site web) et exemples

- modèle de responsabilité entre les modèles de service
- modèles de cloud (hybride, public, privé)

- avec avantage et désavantage de chacun

- diff entre on-premise et cloud privé
- modèle de consommation

- capEX
- opEX


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

