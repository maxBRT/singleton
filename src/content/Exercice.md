# Exercice : Le Jeu

Votre ami a créé un prototype pour un jeu qu'il voudrait publier sur Steam™. Comme il sait que vous êtes de vrai bêtes en programmation, il vous demande de l'aider car il fait face à un bug et il n'arrive pas à le résoudre. 

### Péparation

1. Clonez le dépôt de votre ami.

```bash

    git clone git@github.com:maxBRT/singleton-exercices.git   


```

ou

```bash

    git clone https://github.com/maxBRT/singleton-exercices.git  


```

2. Lancez le projet.

```bash

    cd singleton-exercices  
    mvn clean compile 
    mvn exec:java


```

Le jeu est encore au stade embrionnaire. L'indice de commande vous guidera dans la partie.

### Question 1 : Identification du bug

Vous avez demandé à votre ami de vous expliquer le bug mais il semblerais que ça le rende trop émotif alors vous devrez l'identifier vous-même.

- Lancez le jeu et faites une partie.
- Portez attention à votre score au cours de la partie.
- Lorque la partie se termine, est ce que votre score est correct ? pourquoi ?
- Identifiez la classe qui est responsable du score.
- Identifiez comment cette classe est utilisée.

### Question 2 : Résolution du bug

Le bug pourrait être réglé de plusieurs manières. Si vous réfléchissez au 15 dernière minutes, pouvez-vous penser à un pattron de conception qui pourrait vous aider ?

- Quelle classe devez vous modifier pour vous assurer que le conteur de score soit le meme sur tous les écrans ?
- Est-ce que la modification sur la classe était suffisante ? Si non, quelles modifications devriez-vous faire ?



