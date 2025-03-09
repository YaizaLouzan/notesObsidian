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
| Stockage géo redondant interzone GZRS | Trois zones de disponibilité dans la région primaire et un centre de données unique dans la région secondaire | 16            |
