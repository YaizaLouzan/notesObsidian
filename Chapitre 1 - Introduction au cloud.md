 # Définition
  Le cloud permet d'accéder à des services informatiques via internet. Il repose des serveurs interconnectés dans tout le monde. Offre de la flexibilité et évolutivité sans devoir gérer d'infrastructure physique. 

	Le cloud connaît une croissance continue dans le monde, il est utilisé par les besoins personnels et profesionnels. Les entreprises ont besoin de stocker d'importantes quantités de données et de travailler à distance.
	Le stockage en ligne est une alternative efficace face aux infrastructures limitées et aux serveurs énergivores.

  ## Selon Microsoft
  •Un modèle d’activation d’un accès à la demande à un pool partagé de ressources informatiques configurables : serveurs, réseau, stockage, applications et service.

•Un accès réseau à la demande, omniprésent et pratique.

•Une mise en service et distribution rapides avec un minimum d’effort d’administration ou d’interaction avec le fournisseur de services

**Microsoft** propose d'utiliser la normalisation du NIST comme définition de base du cloud, mais qu'est-ce que le NIST ?

## NIST
*National Institute of Standards and Technology* est une agence gouvernementale américaine. Son rôle est de créer et promouvoir des normes et technologies. 

**Objectifs**: améliorer la sécurité et la compétitivité économique des États-Unis.
**Domaines** : informatique, cybersécurité, cryptographie, ingénierie, métrologie.
Utilisé par Microsoft et d'autres grandes entreprises pour l'innovation et le développement technologique.

# Principaux fournisseurs

- AWS
- Infomaniak
- Microsoft Azure
- Google Cloud
- Kubernetes

# Principes fondamentaux

- **Accès à la demande** : Ressources accessibles instantanément via un portail ou API.
- **Paiement à l'utilisation** : Facturation basée sur la consommation des services.
- **Évolutivité et flexibilité** : Les ressources s'adaptent en temps réel selon les besoins.
- **Maintenance centralisée** : Les fournisseurs gèrent la maintenance et les mises à jour.
- **Accès universel** : Disponible partout avec Internet, favorisant la collaboration et la mobilité.

# Avantages et inconvénients

## Avantages

- Réduction des coûts
	- Uniquement payer les ressources utilisées
- Scalabilité
	- Augmenter ou réduire les ressources selon besoin
- Accès universel
	- Accéder aux données depuis n'import où avec une connexion internet
- Maintenance
	- Le fournisseur les gère
- Haute disponibilité
	- Redondance et sauvegarde dans plusieurs centres de données
- Innovation
	- Accès aux dernières technologies sans gestion supplémentaire

## Inconvénients

- Confidentialité / sécurité
	- S'assurer du respect de la nLPD
- Risque de fuite de données
	- Dépendance de la sécurité du fournisseur
- Problème de connectivité
	- Nécessite une connexion internet
- Performance
	- La latence varie selon la distance et la charge du serveur
- Coûts variables
	- Facturation complexe, difficile à gérer si usage non surveillé
- Migration
	- Transition vers le cloud complexe et chère


# Livraison, tarification et scalabilité

- Livraison
	- On-demand : Ressource disponible immédiatement
	- Préemptive : Allocation anticipée des ressources selon la demande prévue
## Tarification

- Pay-as-you-go : Paiment basé sur l'utilisation réelle
- Abonnement : Coût fixe mensuel ou annuel
- Réservation : réductoion en réservant des ressources à l'avance
## Scalabilité

- Horizontale : Ajouter ou retirer des serveurs pour gérer la charge
- Verticale : Augmenter ou réduire les ressources d'un serveur existant (ex. RAM)

# Emplacement physique

Derrière «le cloud» se trouvent des datacenters physiques, complexes et répartis dans le monde.
Les données et services sont répliqués sur plusieurs serveurs et datacenters pour garantir disponibilité et redondance.

- Datacenter
- Équipement réseau (routeur)
- Alimentation électrique
- Serveurs
- Systèmes de refroidissement
- Sécurité physique (caméras)

# Datacenter en Suisse

- CloudSigma
- Swisscom
## Comment est constitué un datacenter
Un **datacenter** est une infrastructure physique utilisée pour héberger des serveurs, des équipements réseau et des systèmes de stockage. Il est conçu pour assurer la **sécurité, la disponibilité et la performance** des données et services informatiques.

## Niveaux des Datacenters (Tier)

- **Tier 1** : Infrastructure minimale, aucune redondance, temps de disponibilité d’environ 99,671 %.
- **Tier 2** : Ajout de composants redondants (ex. alimentation, refroidissement), disponibilité d’environ 99,741 %.
- **Tier 3** : Infrastructure tolérante aux pannes, redondance complète (N+1), disponibilité d’environ 99,982 %.
- **Tier 4** : Niveau maximal, redondance 2N+1, tolérance aux pannes totale, disponibilité de 99,995 %.
# Hyperscaler - caractéristiques

**Définition** : 
Un **hyperscaler** est un fournisseur de cloud géant, comme **Amazon (AWS), Microsoft (Azure) ou Google (GCP)**, qui gère des **millions de serveurs** répartis dans le monde entier pour offrir des services informatiques ultra-scalables et performants. 

- Grands fournisseurs de services comme Amazon, Facebook, ... 
- Échelle mondiale
	- Expertise et innovation qui font passer le cloud au niveau supérieur
- Gèrent des millions de serveurs et centres de données répartis à travers le monde
- Prix et économies d'échelle significatives
	- Coûts réduits pour les utilisateurs
- Technologies avancées
- Propose des services à valeur ajoutées
	- Gestion de base de données, AI, sécurité
- Offre une suite complète de services informatiques
- Répartis dans le monde entier, assurant redondance et fiabilité
- Se concentrent également sur les besoins régionaux

# Architectures cloud 

## Haute disponibilité

Capable d'un système à fonctionner même en cas de panne, grâce à la répartition des ressources sur plusieurs zones géographiques

## Résilience des données

Capacité d'un système à continuer de fonctionner, ou à se rétablir rapidement, après une panne, une attaque ou un incident technique

## Illustration des 2
Imagine une école avec des copies de ses livres dans plusieurs bibliothèques.  

**Haute disponibilité** : Si une bibliothèque brûle (panne), les élèves peuvent toujours accéder aux livres dans une autre bibliothèque, assurant la continuité.

**Résilience** : Les livres sont régulièrement sauvegardés. Si un livre est endommagé, une copie peut être restaurée rapidement, garantissant qu'aucune donnée n'est perdue.

Ainsi, la haute disponibilité maintient l'accès, et la résilience protège contre la perte de données.

# Région et zone de disponibilité

Les concepts de régions et de zones de dispo sont essentiels dans l'architecture des datacenter pour les services cloud computing. Ils permettent de garantir résilience, sécurité et performance des services cloud à l'échelle mondiale.

## (Régions dans le cloud)

### Région
Zone géographique regroupant plusieurs datacenters, physiquement isolée pour limiter les incidents entre régions.

### Objectifs
Réduire la latence, respecter les lois de résidence des données et offrir une meilleure couverture géographique.

### Régions jumelées
Régions Azure jumelées avec au moins 500 km de distance, assurant la réplication automatique et la récupération rapide en cas de panne.

### Mises à jour
Déployées de manière séquentielle pour minimiser les interruptions de service.
![[Pasted image 20250221073123.png]]

![[Pasted image 20250221073142.png]]

## Zones de disponibilités
-> Avaibility Zone (AZ)

Contient un ou plisuers datacenters isolées au sein d'une même région. Chaque AZ est physiquement distincte et indépendante (électriquement, réseau, systèmes de reffroidissement).

Les AZ sont conçues pour être redondantes et tolérantes aux pannes. Si une AZ subit une panne, les autres AZ de la même région peuvent prendre le relais sans interruption de service -> HAUTE DISPONIBILITÉ

# Cloud souverain

**Définition:**
Un **cloud souverain** est un service cloud dont les **données sont stockées et gérées dans un pays spécifique**, sous le **contrôle des lois locales**, garantissant ainsi **sécurité, confidentialité et indépendance vis-à-vis des acteurs étrangers**. 

-> Localisation spécifique, conformité légale, contrôle renforcé

Le cloud souverain permet auxUS de stocker leurs données sensibles sur leur propre terrain, garantissance la conformité. Il réduit les coûts en mutualisant l'infrastructure et la maintenance avec d'autres entités gouvernementales.
C'est une solution idéale pour les entreprises qui douvent stocker des données sensibles en toute sécurité, comme en Suisse.

Plusieurs fournisseurs suisses se distinguent dans le cloud souverain, ce qui permet aux entreprises suisses de stocker leurs données sensibles sur des servuerus situés en Suisse.

- Swisscom Cloud : Une des plus grandes entreprises de télécommunication en Suisse
- Exoclase : Entreprise suisse de cloud qui propose une plateforme de cloud souverain basée sur OpenStack
- CloudSigma
- ArtMotion
- Nuvia

# OpenStack
OpenStack est une plateforme open source qui permet de créer et de gérer des infrastructures cloud, en offrant des services de calcul, de stockage et de mise en réseau. Elle permet aux utilisateurs de déployer des environnements cloud privés ou publics de manière flexible et évolutive, avec une interface de gestion centralisée. C'est utilisé par de nombreuses entreprises et organisations pour simplifier la gestion de leurs ressources cloud. 

**En gros, c'est une plateforme de cloud sur Infomaniak.**
## (Le cloud et le climat)
En Suisse, Green Datacenter est un exemple de centre de cloud souverain écologique. Ce centre utilise de l'énergie renouvelable à 100% pour alimenter ses servuers, notamment de l'énergie hydroélectrique et solaire.

- Le cloud public ou privé, peut avoir un impact sur l'environnement en raison de la consommation d'énergie nécessaire pour le stockage, le traitement et le transfert de données
- Il est possible de réduire cet impact environnemental en adoptant des pratique écologiques et en utilisant des sources d'énergie renouvelable
- Il es tpossible de choisir des sources d'énergie renouvelables telles que l'énergie solaire ou éolienne pour alimenter les centres de données.
- Enfin, les centres de données doivent être conçus de manière à réduire leur consommation d'énergie, par exemple en utilisant des systèmes de reffroidissement efficaces ou en optimisant l'utilisation de l'espace

# Cloud Microsoft en Suisse
- **Contexte initial** : Microsoft devait se conformer à la loi suisse sur la protection des données, notamment pour la localisation des données.
- **Solution initiale** : Certaines données étaient stockées sur des serveurs en Europe, répondant partiellement aux exigences suisses.
- **Problème** : La loi suisse impose que certaines données sensibles soient exclusivement stockées en Suisse, compliquant la gestion pour les employés.
- **Solution actuelle** : Microsoft propose désormais des serveurs en Suisse, garantissant la conformité légale, réduisant la latence, renforçant la sécurité et répondant aux besoins des clients suisses.

# nLPD
-> Nouvelle Loi sur la Protection des Donnés

Loi fédérale Suisse entrée en vigueur le 1er septembre 2023. Elle s'applique à toutes les entités (publiques ou privées) et dans certains cas aux entités étrangères qui traitent des données personnelles liées à la Suisse. Elle remplace la loi de 1992 (LPD) qui n'était plus adaptée aux technologies modernes (Internet, Cloud, intelligence artificielle, Big Data). 
Donc, on peut les stocker dans des cloud chiffrés.

- **Important** : Une **donnée sensible** est une information personnelle qui, si elle est divulguée, perdue ou mal utilisée, peut porter atteinte à la vie privée, aux droits ou à la sécurité d'une personne. Elles nécessitent des mesurent strictes (analyse d'impact, sécurisation renforcée)
## Préposé des Protection des Données et Transparence

L'**Autorité de protection des données et transparence** intègre la nLPD avec des exigences supplémentaires.
- Publiques et communes: **Toutes** les **institutions publiques** doivent respecter ces règles.
- Sous-traitants : Si l'entité traite des données pour le public, elle doit respecter ces règles
- PPDT (préposé à la protection des données)



## Droits des citoyens
Les 2 lois précédentes incluent des droits des citoyens : 

### nLPD
**- Droit à l'information**
	- Toute personne a le droit de savoir quelles données personnelles sont collectées, pour quelles finalités et par qui.
**- Droit d'accès**
	- Chaque citoyen peut demander gratuitement l’accès à ses données personnelles détenues par une entreprise ou une organisation. L'entité concernée doit répondre dans un délai de 1 mois.
**- Droit de rectification**
	- Si des données sont inexactes ou incomplètes, la personne concernée peut exiger leur correction.
**- Droit à l'effacement**
	- Dans certaines conditions, un individu peut demander la suppression de ses données personnelles, par exemple si elles ne sont plus nécessaires ou si le consentement est retiré.
**- Droit d'opposition et limitation du traitement**
	- Une personne peut s’opposer au traitement de ses données si cela porte atteinte à ses intérêts ou libertés. Elle peut aussi demander la limitation du traitement dans certains cas.
**- Droit à la portabilité des données**
	- Les citoyens peuvent demander que leurs données personnelles soient transmises à un autre prestataire dans un format structuré et couramment utilisé
**- Droit à ne pas être soumis à une décision automatisée**
	- Si une décision impactant une personne (par ex., un refus de crédit) est prise uniquement par un algorithme sans intervention humaine, elle peut demander une explication et contester cette décision.

En cas de violation des droits, un citoyen peut saisir le Préposé fédéral à la protection des données et à la transparence (**PFPDT**), qui peut mener une enquête et prendre des mesures.

### PPDT
La **PPDT** régit la protection des données au niveau **cantonal** et concerne les institutions publiques (administrations cantonales et communales). Les droits sont similaires à ceux de la nLPD, avec un accent particulier sur :

- **La transparence de l'administration publique** : les citoyens peuvent demander l’accès aux documents administratifs.
- **La protection des données personnelles traitées par les autorités cantonales et communales**.
- **Le recours à un médiateur ou préposé cantonal** en cas de litige.

📍 **À noter :** La PPDT peut varier légèrement selon les cantons, bien que les principes de base restent alignés sur la nLPD.

# Niveaux de localisation des datacneters chez Microsoft

Les centres de données Microsoft sont certifiés.
## Global
•Données stockées dans des centres à travers le monde.
•Haute résilience, disponibilité, et performances optimisées.
•Conformité pour les organisations internationales.

## Local
- Données stockées dans une région spécifique.
- Respect des lois locales et réduction de la latence.
- Conformité avec les réglementations locales.
## Souverain
- Cloud dédié et isolé
- pour gouvernements / secteurs sensibles.
- Souveraineté totale des données
- sécurité et conformité maximales.
