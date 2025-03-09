# Azure Arc
**Azure Arc est une technologie qui permet d’étendre Azure partout.**

- Dans ton **datacenter privé** (serveurs physiques ou machines virtuelles)
- Dans **d’autres clouds** (AWS, Google Cloud)
- Dans des **clusters Kubernetes** ou des bases de données SQL ailleurs

Grâce à **Azure Arc**, tu peux **gérer toutes ces ressources comme si elles étaient dans Azure**, **même si elles ne le sont pas** !

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

# Outils de supervision Azure

## Azure Advisor

Analyse les ressources Azure déployées et formule des recommandations basées sur les meilleures pratiques en vue d'optimiser les déploiements Azure

1. Fiabilité
2. Sécurité
3. Performances
4. Coût
5. Excellence opérationnelle

En résumé :

- Obtenez des suggestions de meilleures pratiques proactives, exploitables et personnalisées
- Améliorez les niveaux de performances, la sécurité et la disponibilité de vos ressources
- Identifiez les opportunités de réduire vos coûts Azure

## Azure Service Health
c'est un ensemble de services qui vous informent :

De l’état général d’Azure, de l’état du service susceptible de vous impacter et de l’état d’une ressource spécifique qui vous impacte

### Azure Status
Vue globale de l’intégrité des services Azure dans l’ensemble des régions Azure

### Service Health
Vue axée uniquement sur les services et régions que vous utilisez
Si un service rencontre un problème dans une région que vous n’utilisez pas, il n’apparaîtra pas ici

## Azure Monitor
Plateforme permettant de collecter des données sur vos ressources, d’analyser ces données, de visualiser les informations. Permet de superviser les ressources Azure, vos ressources locales et même les ressources multiclouds telles que les machines virtuelles hébergées avec un autre fournisseur de cloud.

- Application Insights
- Log Analytics
- Alertes intelligentes
- Actions d’automatisation
- Tableaux de bord personnalisés

