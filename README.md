# koha-plugin-data-inconsistencies
Extension SearchForDataInconsistencies pour le SIGB Koha

Cette extension permet d'identifier les incohérences dans la base de données pour assurer la qualité des informations.

Plusieurs types d'incohérences peuvent être identifiées tels :

    - Exemplaires sans bibliothèque propriétaire ou dépositaire 
    - Notices d'autorité sans type d'autorité valide 
    - Notices bibliographiques et exemplaires sans type de document ou avec un type de document non valide
    - Valeurs dans les zones limitées à des valeurs autorisées 
    - Notices bibliographiques sans titre
    - Utilisateurs trop jeunes ou trop âgés pour leur catégorie 
    - Boucles de relations entre utilisateurs

**Attention!**

L'utilisation de cette extension requiert actuellement la patch 36027. Pour l'appliquer, vous pouvez utiliser la commande ```git bz apply 36027```.

## Générer le rapport

Pour atteindre la page de génération du rapport, utiliser l'action <b>Exécuter l'outil</b> de l'extension SearchForDataInconsistencies dans le tableau des extensions.

Le bouton <b>Vérifier les incohérences des donnéees</b> permet alors de générer le rapport. 

### Modifier les données 

Dans la page du rapport, pour chaque donnée incohérente, un bouton permet d'accéder à la page de modification de la notice, de l'exemplaire, de l'authorité ou de l'utilisateur,
selon le type d'incohérence. 
