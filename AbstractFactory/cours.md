### Le pattern Abstract Factory
Le but : Avoir des familles d'objet autour d'une classe abstraite. Pas besoin de connaitre la classe concrète pour créer les objets.
Classe abstraite générique et des sous classe concrète.

![Alt text](<../consoleApp/template pattern.png>)

pointiller :  relation ou l'autre ne peut exister sans celui sur lequel il dépend
la classe abstraite n'a pas besoin de savoir ce qui est créer, c'est l'interface qui s'en charge.
La classe concrète prend en paramaètre une instance qui va implémenter une interface.