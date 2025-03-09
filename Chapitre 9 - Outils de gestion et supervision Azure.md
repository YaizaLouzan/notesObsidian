# Azure Arc
## Principales fonctionnalités
- Gestion de serveurs hybrides
- Gestion des clusters Kubernetes
- Services de données Azure
- Gouvernance et conformité
- Automatisation

## C'est quoi ?
Plateforme de gestion unifiée pour serveurs, Kubernetes et services de données.
Étend les capacités d'azure aux environnements multi-cloud, sur site et é périphérie

# Azure Ressource Manager (ARM)
Service de déploiement et de gestion d'Azure. Il permet de déployer, gérer et surveiller les ressources Azure de manière cohérente.

- Permet de créer, configurer, gérer et supprimer des ressources et groupes de ressources
- Permet d'organiser les ressources
- Contrôle l'accès et les ressources
- Permet l'automatisation à l'aide de différents outils et kits de développement logiciel
- Stocke les disposition dans les fichiers JSON

## Gouvernance et conformité
Les modèles ARM (Azure Resource Manager) sont des fichiers JSON (JavaScript Object Notation) utilisés pour créer et déployer une infrastructure Azure sans devoir écrire de commandes de programmation.

- Syntaxe déclarative
- Résultats reproductibles
- Orchestration
- Fichiers modulaires
- Validation intégrée
- Code exportable

## Déployer les ressources d'application
Azure Resource Manager vous permet de déployer plusieurs fois votre application avec l’assurance que vos ressources seront déployées de manière cohérente

Vous définissez l’infrastructure et les dépendances de votre application dans un seul modèle déclaratif

Ce modèle est suffisamment flexible pour être utilisé dans tous vos environnements : environnements de test, temporaires ou de production

Si vous créez une solution depuis la Place de marché Azure, la solution inclura automatiquement un modèle que vous pouvez utiliser pour votre application

## Organiser les ressources

Azure Resource Manager vous aide à gérer et à visualiser les ressources dans votre application

Vous n’avez plus à déployer des composants de votre application séparément, puis à les assembler manuellement

Vous intégrez les ressources présentant un cycle de vie commun dans un groupe de ressources, qui peut être déployé ou supprimé dans une seule action

Vous pouvez voir les ressources qui sont liées par une dépendance

Vous pouvez appliquer des étiquettes aux ressources afin de les classer pour des tâches de gestion telles que la facturation

## Contrôler l’accès aux ressources

Avec Azure Resource Manager, vous pouvez contrôler qui, au sein de votre organisation, peut agir au niveau des ressources

Vous gérez les autorisations en définissant des rôles et en ajoutant des utilisateurs ou des groupes aux rôles

Pour les ressources critiques, vous pouvez appliquer un verrou explicite qui empêche les utilisateurs de supprimer ou de modifier la ressource

Azure Resource Manager enregistre toutes les actions des utilisateurs afin que vous puissiez les contrôler

Pour chaque action, le journal d’audit contient des informations sur l’utilisateur, l’heure, les événements et le statut