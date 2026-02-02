## La solution

Souvent, il y a quelque chose de beau dans les patrons de conception. Ce petit sentiment que tout est en ordre et que le travail est bien fait. Avec le singleton, c'est... un peu différent. Ce patron donne plutôt l'impression d'être une espèce de hack pour contourner les restrictions du langage. 

La solution qu'il propose aux deux problèmes précédemment cités est la suivante :

On cache le constructeur de la classe derrière un champ privé, la classe garde une référence statique vers elle-même et on expose une méthode publique qui retourne cette instance (ou la crée au premier appel).


