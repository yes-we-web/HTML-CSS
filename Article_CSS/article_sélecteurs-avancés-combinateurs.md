Bonjour à tous  :wave: .
On espère que vous allez bien :bangbang:

Aujourd'hui on va vous présenter :



# **_Les sélecteurs avancés_** :

(eh oui, encore des noms barbares mais ça va aller!)

Les sélecteurs avancés ont le pouvoir de sélectionner tous les éléments d’une page HTML, 
sélectionner un élément par rapport à son parent ou encore sélectionner un élément selon la valeur de son attribut.
Il en existe plusieurs mais nous allons (pour l'instant) voir les principaux (les plus utilisés).




## **_Le sélecteur attribut_** :

Il permet de cibler un élément ou une valeur donnée d'un attribut.

Il existe plusieurs attributs, nous allons en voir quelqu'un ensemble :

* **[attr=valeur]** : ceci permet de cibler un élément qui possède un attribut dont la valeur est exactement ce que l'on tape.

Par exemple:
```
p[href="url entier de ce que l'on veut]

on cible donc tous les p qui possédent un href avec le lien entier.
```
* **[attr^=valeur]** : ceci permet de cibler un élément qui possède un attribut dont la valeur commence par le mot que l'on veut.

Par exemple:
```
p[class^="promo"]

on cible donc toutes les classes qui doivent se nommer ( ou du moins le début ) par "promo",
imaginons qu'une classe s'appelle "promo-2-Yes-We-Web", alors elle sera ciblée car elle commence par "promo".
```
* **[attr$=valeur]** : ceci permet de cibler un élément qui possède un attribut dont la valeur finit par le mot que l'on veut.

Par exemple:
```
p[href$=".com"]

on cible donc tout les p qui ont un href finissant par ".com".
```

On va s'arreter là pour l'instant sinon on va faire un article spécifiquement sur le sélecteur attribut :sweat_smile: ,
si vous voulez en savoir plus sur ce qu'on peut utiliser sur le sélecteur attribut: nous vous invitons à allez voir juste [ici.](https://developer.mozilla.org/fr/docs/Web/CSS/S%C3%A9lecteurs_d_attribut)



## **_Le sélecteur de voisin direct_** :     ( A + B ) 

Ce sélecteur permet de sélectionner un élément uniquement s'il suit l'élément donné et que les deux éléments sont les fils d'un même élément parent. Un combinateur est utilisé ici mais nous le verront juste en dessous.

Exemple:
```
div + p

Ceci permet de cibler n'importe quel p qui suit immédiatement n'importe quelle div
```


## **_Le sélecteur de voisin_** :     ( A ~ B )

Ce sélecteur est proche du sélecteur voisin direct mais largement moins strict. Alors qu'un sélecteur de voisin direct (dit adjacent) ne cible que le premier élément immédiatement de l'élément donné, celui-ci vite plus large. Il sélectionne n'importe quel élément, du moment qu'il le suit.

Exemple:
```
p ~ span

permet de cibler tout les élements span qui suivent ( immédiat ou pas ) un élément p et qui ont le même élément parent.
``` 

Pour une fois que le voisin sert à quelque chose :laughing:



## **_Les sélecteurs d'éléments fils_** :     ( A > B )

Ce sélecteur permet de sélectionner les éléments qui sont des fils direct d'un élément donné.

Exemple:
```
ul > li

permet de cibler tous les li qui sont directement situés sous un élément ul.
```



## **_Les sélecteurs d'éléments descendants_** :     ( A B )

Ce sélecteur permet de sélectionner les éléments qui sont descendants ( pas nécessairement des fils directs ) d'un élément donné.

Exemple:
```
div span

permet de cibler n'importe quel élément span situé à l'intérieur de n'importe quelle div.
```

On vous a montré un étendu des principaux sélecteurs avancés :dizzy_face: ,
on va passer maintenant au combinateurs. :kissing_closed_eyes:



# **_Les combinateurs_** :

Les combinateurs, rien de plus facile :grin: ( oui :bangbang oui :bangbang: On a bien dit **FACILE** ça existe ), on en a vu juste au dessus avec les sélecteurs avancés.
Les combinateurs les plus importants sont:

* Le combinateur `+` permet de sélectionner les noeuds qui suivent immédiatement un élément donné.
* Le combinateur `~` permet de sélectionner les noeuds qui suivent un élément et qui ont le même parent.
* Le combinateur '>' permet de sélectionner les noeuds qui sont fils direct d'un élément donné.
* Le combinateur '(espace)' permet de sélectionner les noeuds qui sont fils direct d'un élément donné.
* Le combinateur '||' permet de sélectionner les noeuds qui appartiennent à une colonne.

Il y a tellement de combinateurs si vous l'auriez compris, le nom peut être effrayant mais ce sont nos amis :innocent:

Voilà, vous pouvez soufflé, nous venons de conclure notre article CSS.
On reste à votre disposition si vous avez besoin d'autres explications ou des questions. :smile:



Toute la Team vous remercie. :wave:

Ahmad, Céline, Louis, Antoine, Amandine.


:point_right: [Article Précedent : Cascade et Héritage en CSS](article_héritage-cascade.md) :point_left:

:point_right: [Article Suivant : Responsive Design](article_responsive.md) :point_left:
