## La solution

Le Singleton résout ces deux problèmes d’une façon élégante même si il est parfois controversé. Les avis varient entre un “Hack” astucieux et un patron légitime. Une chose qui est sure, c’est que le patron fonctionne. 

La solution repose sur trois principes fondamentaux :

**Premièrement**, on rend le constructeur privé. En faisant cela, on empêche complètement la création d'instances depuis l'extérieur de la classe. Plus personne ne peut faire : 
`new Singleton()`, cette porte est fermée à clé.

**Deuxièmement**, la classe conserve une référence statique vers sa propre instance. C'est ici que l'unique instance sera stockée, accessible uniquement à l'intérieur de la classe elle-même. Cette référence statique appartient à la classe, pas aux instances individuelles.

**Troisièmement**, on expose une méthode publique qui contrôle l'accès à l'instance. Cette méthode, généralement appelée `getInstance()`, fait office de constructeur public. Mais contrairement à un vrai constructeur, elle ne crée pas systématiquement un nouvel objet. Au premier appel, elle crée l'instance et la stocke. Aux appels suivants, elle retourne simplement cette même instance déjà créée.

**En résumé :** le Singleton transforme le problème en avantage. Au lieu de laisser tout le monde créer des instances, il centralise ce contrôle à l'intérieur de la classe elle-même, garantissant ainsi qu'une seule instance existe et que l'accès à celle-ci soit à la fois global et sécurisé.

```java

    UserService s1 = new UserService();

    UserService s2 = new UserService(); // différent

    // Avec un Singleton, au contraire, 
    // la méthode getInstance() retourne toujours la même instance.
    
    UserService s1 = UserService.getInstance();

    UserService s2 = UserService.getInstance(); // même objet

    // Les deux variables pointent donc vers le même objet.
    s1 === s2 => true


```
