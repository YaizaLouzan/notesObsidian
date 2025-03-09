Capacité de traiter des données et d'exécuter des applications

- Serverless
Le développeur ne gère que le code de l’application, le fournisseur provisionne, dimensionne et gère les serveurs sans intervention manuelle.

Vous n'avez pas à vous soucier des serveurs, des machines ou de la gestion des ressources, tout est automatisé

- Bare Metal
Serveurs physiques dédiés, offrant des performances maximales tout en bénéficiant de la flexibilité du cloud. **Exemples** : AWS Bare Metal Instances, IBM Cloud Bare Metal Servers

- Conteneurs
Des unités légères qui encapsulent les applications et leurs dépendances pour un déploiement rapide et une grande portabilité.

Exemples : Amazon ECS, Google Kubernetes Engine.

- Machines Virtuelles
Exemples : Amazon EC2, Microsoft Azure VMs, Google Compute Engine.

|**Option de calcul**|**Modèle de cloud**|**Explication**|
|---|---|---|

|   |   |   |
|---|---|---|
|🖥 **Machines Virtuelles (VMs)**|IaaS (Infrastructure as a Service)|Le fournisseur cloud gère le matériel et la virtualisation, mais l’utilisateur gère le système d’exploitation et les applications. Ex : AWS EC2, Azure VM.|

|   |   |   |
|---|---|---|
|📦 **Conteneurs (Docker, Kubernetes, etc.)**|IaaS / PaaS|Sur IaaS, l’utilisateur gère l’infrastructure et l’orchestration (ex: Kubernetes sur AWS). Sur PaaS, le fournisseur simplifie la gestion (ex: Google Kubernetes Engine).|

|   |   |   |
|---|---|---|
|⚡ **Serverless (FaaS - Function as a Service)**|PaaS / FaaS|L’utilisateur écrit du code sans gérer les serveurs. Ex : AWS Lambda, Google Cloud Functions.|

|   |   |   |
|---|---|---|
|🏗 **PaaS (Platform as a Service)**|PaaS|Plateforme prête à l’emploi pour développer et héberger des applications, sans gérer les serveurs. Ex : Google App Engine, Heroku.|

|   |   |   |
|---|---|---|
|🔧 **Bare Metal**|IaaS|Serveur physique dédié sans virtualisation. Utile pour des charges lourdes comme les bases de données critiques.|

|   |   |   |
|---|---|---|
|☁️ **Cloud hybride**|Mix de IaaS, PaaS et FaaS|Combine plusieurs modèles pour équilibrer coût, performance et sécurité.|

