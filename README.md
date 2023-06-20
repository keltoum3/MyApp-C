# MyApp-C

Prise de note du cours:

Design Pattern C#: (fichier .md à mettre dans le git)

3 façon d'appréhender les problèmes

Faires des choses très général permet la réutilisabilité facilement

git:

-git init
-git remote add origin git@github.com:keltoum3/MyApp-C.git
-git branch -M main
-git push -u origin main


-Les design patterns(patterns de conception):

Le design pattern permet notamment d'accélérer le processus de développement. Cela aide à gagner du temps sans avoir à réinventer des modèles chaque fois qu'un problème apparaît. Basé sur les bonnes pratique de la programmation orienté objet. Abstraire la conception d'objet.

Présenation des design patterns 
Les design patterns:
descritpion des patterns:
-nom
-direction
-exemple de code sous forme de diagramme UML
-La structure standard (abstraite)
-Un exemple de code


Cas concret:
Nous allons prendre en exemple le cas d'une société qui vend des véhicules en ligne 

Important:
Sélectionner et utiliser un pattern qui peut répondre à la problématique que l'on rencontre

## Première grande famille de design pattern: 
Les patterns de construction:
Le but est de simplifier la création d'objet. Ce pattern permet de rendre abstraite la création d'objet et de la standardisé peu importe. favoriser l'usage d'interface pour intéragir avec les objets. ( pattern singleton). Une classe avec une seule instance. Les clients de la classe ne sont pas au courant qu'ils utilisent une seule instance de classe. On cache la création d'objet au client. Modèle abstrait identique mais instanciation différentes.

### Le pattern Abstract Factory
Le but : Avoir des familles d'objet autour d'une classe abstraite. Pas besoin de connaitre la classe concrète pour créer les objets.
Classe abstraite générique et des sous classe concrète.

![Alt text](<template pattern.png>)

pointiller :  relation ou l'autre ne peut exister sans celui sur lequel il dépend
la classe abstraite n'a pas besoin de savoir ce qui est créer, c'est l'interface qui s'en charge.
La classe concrète prend en paramaètre une instance qui va implémenter une interface.

### Pattern builder
Permt d'abstraire la conception d'objets complexes de leur implémentation de sorte qu'un client puisse créer des objets complexe sans avoir à se préoccuper des différences d'implémentation.

![Alt text](<diagramme pattern builder.png>)

Pourquoi utiliser ce pattern: 
-le client à besoin de construire des objets sans connaitre leur implémentation
-Un client à besoin de construire des objets complexes ayant plusieurs représenations ou implémentations

