## Dictionnaire de données en amont de la modélisation

User

|Nom|Type|Taille|Description|
|-|-|-|-|
|num_user|Entier|-|Numéro permettant d'identifier un utilisateur|
|name|Chaîne de caractères|100|Titre du podcast|
|password|chaîne de caractères|255|Mot de passe de l'utilisateur|
|created_at|Date|-|Date de création|
|updated_at|Date|-|Date de mise à jour|


Product

|Nom|Type|Taille|Description|
|-|-|-|-|
|num_product|Entier|-|Numéro permettant d'identifier un produit|
|name|ChaÎne de caractères|100|Nom du produit|
|quantity|Texte|100|Stock actuel pour le produit|
|status|Texte|100|Statut du produit (0 = archivé/hors-ligne, 1 = en ligne). Un produit ne doit pas pouvoir être supprimé dès lors qu'il fait partie d'une commande. Si on souhaite le retirer de la vente, on l'archivera.|
|created_at|Date|-|Date de création|
|updated_at|Date|-|Date de mise à jour|



Catégory

|Nom|Type|Taille|Description|
|-|-|-|-|
|num_category|Entier|-|Numéro permettant d'identifier une catégorie|
|name|Chaîne de caractères|100|nom de la catégorie|
|created_at|Date|-|Date de création|
|updated_at|Date|-|Date de mise à jour|


Tag

|Nom|Type|Taille|Description|
|-|-|-|-|
|num_tag|Entier|-|Numéro permettant d'identifier l'étiquette|
|name|Chaîne de caractères|100|nom de l'étiquette|
|created_at|Date|-|Date de création|
|updated_at|Date|-|Date de mise à jour|


Order

|Nom|Type|Taille|Description|
|-|-|-|-|
|num_order|Entier|-|Numéro permettant d'identifier une commande|
|num_invoice|Chaîne de caractères|100|Numéro de facture (une fois la commande validée)|
|status|Chaîne de caractères|100|Etat de la commande ('En panier', 'En cours de traitement' (une fois validé par l'utilisateur), 'Validé', 'En cours de livraison' et 'Livré')|
|created_at|Date|-|Date de création|
|updated_at|Date|-|Date de mise à jour|



## Evolution du dictionnaire de données après le MPD

User

|Nom|Type|Taille|Description|
|-|-|-|-|
|id|BIGINT UNSIGNED|-|ID de l'utilisateur|
|name|VARCHAR|100|Nom de l'utilisateur|
|password|VARCHAR|100|Mot de passe de l'utilisateur|
|created_at|TIMESTAMP|-|Date de création|
|updated_at|TIMESTAMP|-|Date de mise à jour|


Product

|Nom|Type|Taille|Description|
|-|-|-|-|
|id|BIGINT UNSIGNED|-|ID du produit|
|name|VARCHAR|100|nom du produit|
|quantity|BIG INT UNSIGNED|100|Stock actuel du produit|
|status|BIG INT UNSIGNED|100|Statut du produit (0 = archivé/hors-ligne, 1 = en ligne). Un produit ne doit pas pouvoir être supprimé dès lors qu'il fait partie d'une commande. Si on souhaite le retirer de la vente, on l'archivera.|
|created_at|TIMESTAMP|-|Date de création|
|updated_at|TIMESTAMP|-|Date de mise à jour|


Catégory

|Nom|Type|Taille|Description|
|-|-|-|-|
|id|BIG INT UNSIGNED|-|ID de la catégorie|
|name|VARCHAR|100|titre de la catégorie|
|created_at|TIMESTAMP|-|Date de création|
|updated_at|TIMESTAMP|-|Date de mise à jour|


Tag

|Nom|Type|Taille|Description|
|-|-|-|-|
|id|BIG INT UNSIGNED|-|ID du tag|
|name|VARCHAR|100|titre du tag|
|created_at|TIMESTAMP|-|Date de création|
|updated_at|TIMESTAMP|-|Date de mise à jour|


Order

|Nom|Type|Taille|Description|
|-|-|-|-|
|id|BIGINT UNSIGNED|-|ID de la commande|
|num_invoice|VARCHAR|100|Numéro de facture (une fois la commande validée)|
|status|VARCHAR|-|Etat de la commande ('En panier', 'En cours de traitement' (une fois validé par l'utilisateur), 'Validé', 'En cours de livraison' et 'Livré')|
|created_at|TIMESTAMP|-|Date de création|
|updated_at|TIMESTAMP|-|Date de mise à jour|

