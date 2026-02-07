Le Singleton est un patron de conception de type créationnel.
Les patrons créationnels ne s’occupent pas du comportement des objets ni de leurs interactions, mais plutôt de la façon dont ils sont créés en mémoire.
Ils contrôlent donc comment et combien d’instances peuvent exister.
Le Singleton applique cette idée de manière stricte : il garantit qu’une classe ne possède qu’une seule instance pendant toute la durée de vie de l’application, tout en offrant un point d’accès global et centralisé pour y accéder.

L’intention du Singleton repose sur trois besoins principaux:

- D’abord, la cohérence de l’état.
- Ensuite, un accès global **et** sécurisé.
- Enfin, il y a la question des performances.

Maintenant, dans les applications réelles, on utilise surtout les Singletons pour des services techniques globaux, plutôt que pour de la logique métier.

Un exemple très courant de Singleton, c’est la configuration globale de l’application.
Elle regroupe toutes les informations importantes : variables d’environnement, paramètres système, clés API, ports réseau, options de démarrage, etc.
Cette configuration est généralement chargée une seule fois au lancement, puis partagée en lecture seule dans toute l’application.
Comme ça, tous les modules utilisent exactement les mêmes valeurs.
Ça évite de recharger la configuration plusieurs fois,  ça garantit la cohérence des paramètres et ça améliore les performances.
D’ailleurs, la plupart des frameworks backend comme Spring Boot, Django ou Node.js fonctionnent déjà comme ça : la configuration est chargée au démarrage puis partagée partout dans l’application.