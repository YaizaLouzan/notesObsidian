# Compte de stockage
Un **compte de stockage Azure** est une ressource cloud dans laquelle on peut stocker des données. Il sert de conteneur pour plusieurs types de services de stockage, comme les **blobs**, les **fichiers**, les **queues** et les **tables**. Il permet de gérer les données de manière sécurisée et accessible partout dans le monde via Internet.

Principales caractéristiques:

- Offre un nom d'espace unique pour vos données sur Stockage Azure (cf image point de terminaison ci-dessous).
- Accessible partout dans le monde via les protocoles HTTP ou HTTPS
- Les données stockées dans ce compte sont sécurisées, hautement disponibles, durables et évolutives


# Redondance au stockage
Pour garantir la disponibilité des données, Azure offre plusieurs options de redondance :

- **LRS (Locally Redundant Storage)** : Réplication dans un seul centre de données, pour des besoins locaux.
    
- **GRS (Geo-Redundant Storage)** : Réplication dans un autre centre de données situé dans une autre région géographique pour plus de sécurité.
    
- **ZRS (Zone-Redundant Storage)** : Réplication dans plusieurs zones d'une même région Azure pour une disponibilité élevée.


| Configuration de la redondance        | Déploiement                                                                                                   | Disponibilité |
| ------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------- |
| Stockage localement redondant LRS     | Centre de données unique dans la région primaire                                                              | 11 neuf       |
| Stockage redondant interzone ZRS      | Trois zones de disponibilité dans la région primaire                                                          | 12 neuf       |
| Stockage géo redondant GRS            | Centre de données unique dans les régions primaire et secondaire                                              | 16 neuf       |
| Stockage géo redondant interzone GZRS | Trois zones de disponibilité dans la région primaire et un centre de données unique dans la région secondaire | 16 neuf       |
## Nombre de neuf
Le terme "9" se réfère au niveau de **disponibilité** ou de **durabilité** garanti par un fournisseur. Il est généralement exprimé en pourcentage avec des "9" répétés, comme **99,9%** ou **99,9999%**, et représente une promesse de fiabilité du service.

Explication des **"9" en redondance** :

Le nombre de 9 correspondent à un pourcentage où le serveur est fonctionnel.

EXEMPLE 
S'il y a 5 neufs, on parle de 99,999% car ça fait 5 neuf en tout

CALCUL

5 neuf correspondent à 99,999% (temps serveur fonctionnel)

	0.001%   (temps serveur non fonctionnel)
car 100% - 99,999% = 0,001%
Pour savoir combien de temps un serveur peut rester indisponible.

365 [jours] * 24 [heures] * 60 [minutes] = 525 600 minutes 
-> 525 600 * (0.001/100) = 5.256 minutes

# Services de stockage
## Conteneur de stockage - blob
Optimisé pour stocker des quantités massives de **données non structurées**

Principalement utilisé:

- **Stockage d’objets multimédias** : Images, vidéos, fichiers audio pour des applications web ou mobiles.
    
- **Sauvegarde et restauration** : Fichiers de sauvegarde, bases de données ou disques virtuels.
    
- **Big Data et analytique** : Stockage de données non structurées pour des traitements et analyses massives.
    
- **Archivage** : Conservation de données sur le long terme avec le niveau Archive.

## Stockage sur disque
Service cloud de Microsoft Azure qui fournit des disques virtuels persistants pour les VM et les autres services Azure. Il est utilisé principalement pour **attacher un espace de stockage durable aux VM**

## Azure Files
Service de stockage dans le cloud qui permet de créer et de gérer des **partages de fichiers** accessibles via les protocoles SMB et NFS. Il s'agit d'une solution entièrement managée qui offre les avantages du stockage de fichiers traditionnels avec la flexibilité du cloud. Ce service permet :

- Partage de fichiers SMB et NFS
- Accès à distance
- Intégration avec Azure AD ou AD DS
- Résilience et disponibilité
- Snapshots
- Sauvegardes et restaurations

## Stockage de table
Service qui stocke des données **NoSQL structurées** dans le cloud, fournissant un magasin de clés/attributs avec une conception sans schéma.

## Azure data Lake
Grands volumes de données dans leur forme originale

## Azure NetApp Files

## Azure File Sync
Service permettant d'archiver plusieurs partages dans un serveur Windows on-permise ou dans une VM cloud
## Azure Stack Edge

## Azure Data Box

## Azure Elastic SAN

## Stockage de conteneur Azure

## Azure Storage Actions