# Azure Arc
**Azure Arc est une technologie qui permet d’étendre Azure partout.**

- Dans ton **datacenter privé** (serveurs physiques ou machines virtuelles)
- Dans **d’autres clouds** (AWS, Google Cloud)
- Dans des **clusters Kubernetes** ou des bases de données SQL ailleurs

Grâce à **Azure Arc**, tu peux **gérer toutes ces ressources comme si elles étaient dans Azure**, **même si elles ne le sont pas** !

# Azure Ressource Manager (ARM)
Service de déploiement et de gestion d'Azure. Il **permet de déployer, gérer et surveiller les ressources Azure** de manière cohérente.
- Stocke les disposition dans les fichiers JSON

# Outils de supervision Azure

## Azure Advisor

Analyse les ressources Azure déployées et formule des recommandations basées sur les meilleures pratiques en vue d'optimiser les déploiements Azure

1. Fiabilité
2. Sécurité
3. Performances
4. Coût
5. Excellence opérationnelle
## Azure Service Health
C'est un ensemble de services qui vous informent de l’état général d’Azure, de l’état du service susceptible de vous impacter et de l’état d’une ressource spécifique qui vous impacte

### Azure Status
Vue globale de l’intégrité des services Azure dans l’ensemble des régions Azure

### Service Health
Vue axée uniquement sur les services et régions que vous utilisez.
Si un service rencontre un problème dans une région que vous n’utilisez pas, il n’apparaîtra pas ici

## Azure Monitor
Plateforme permettant de collecter des données sur vos ressources, d’analyser ces données, de visualiser les informations.
# Azure Cloud Shell
Terminal basé sur un navigateur qui fournit une expérience d'interpréteur de commandes authentifiée et préconfigurée pour gérer les ressources Azure
# Azure CLI
Collecte les données de télémétrie par défaut. Microsoft agrège les données collectées pour identifier les modèles d'utilisation, identifier les problèmes courants et améliorer l'expérience Azure CLI.