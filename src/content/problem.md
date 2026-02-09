## Les problèmes qu'il règle

1. **Il s'assure qu'une classe à une seul instance** 

Pour comprendre comment le singleton fonctionne, il faut d'abord comprendre comment fonctionne un constructeur.

Lorsqu'on appelle un constructeur, on lui demande implicitement : « Crée-moi une nouvelle instance de cette classe », ce qui est généralement ce que l'on veut faire !

En revanche, ce n'est parfois pas ce que l'on souhaite, par exemple lorsque l'objet en question contient des données ou des états qui doivent être partagés à travers l'application.

Si ces données ne sont qu'en lecture seule, ce n'est pas si problématique. Cependant, dans une application complexe où les états et les données changent constamment, il faut une solution plus fiable !

2. **Il donne un point d'accès global**

Certains langages nous permettent de définir des variables globales qui peuvent être accédées de n'importe où dans le code. Cette pratique n'est pas très bien perçue (avec raison) puisque, bien qu'elle donne un point d'accès global à notre objet, elle ne lui offre aucune protection. Cette variable pourrait être écrasée par n'importe quelle autre partie de notre programme.

Donc, lorsqu'on dit « donner un accès global à un objet », on sous-entend plutôt : donner un point d'accès global et sécurisé !


