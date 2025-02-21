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

# Hyperscaler - caractéristiques

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

Capacité d'un système 