```java


 public final class Singleton {
    
     private static Singleton instance;
     public String value;
     
     // Le constructeur est privé donc, 
     // seulement accessible à l'intérieur de la classe

     private Singleton(String value) {
         this.value = value;
     }

     
     // Cette méthode fait office de 
     // constructeur public. Cependant, elle 
     // ne retourne pas un nouvel objet a chaque appel.
     // Elle retoure l'insance qui est cacher 
     // à l'intérieur de cette classe

     public static Singleton getInstance(String value) {
         if (instance == null) {
             instance = new Singleton(value);
         }
         return instance;
     }
 }


```
