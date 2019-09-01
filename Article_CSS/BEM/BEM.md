## Introduction au B.E.M en CSS.

Dans cet article nous allons présenter ce qu'est le *B.E.M*  et expliquer a quoi ça sert, si vous avez des bases en CSS vous n'aurez pas trop de difficultés a comprendre le fonctionnement et vous trouverez surement ça trés utile ;) .

# Qu'est ce que c'est ?

Tout dabord *BEM* est une abréviation pour Blocks-Elélments-Modifiers ,Blocs-Eléments-Modificateurs en francais.
Pour faire simple c'est une méthodologie qui consiste a envisager la composition d'une page web en 2 composant bloc et élément.
Cette méthodologie est par Yandex (plus grand moteur de recherche russophone du monde) en 2006 et devennue open source en 2010 ,pourquoi? principalement car :
*Toute modification du code d'une page affectait le code des autres pages.
*Il était difficile de choisir des noms de classe.

-**Le bloc** est le composant parent qui peut contenir un ou plusieur élements par exemple : un menu ,un footer(pied de pages), un header (haut de page).En Html les bolcs sont représenté par l'attribut *class* .

-**L'élément** quant a lui est  un composant appartenant à un bloc. *L'élément* est considéreé  comme étant l'enfant d'un bloc.Un élément fait toujours partie d'un bloc,et pas d'un autre élément.

    par exemple : le titre d'un bloc, une page d'un menu.

-Et **le modificateur** alors ? Il est là pour définir l'apparence, l'état ou le comportement d'un composant. Il se modifie en fonction du contexte de la page ou d'une action de l'utilisateur. Il peut aussi bien être appliqué à un bloc qu'à un élément.Par exemple : un fond de couleur différente pou une page spécifique, un élément rendu visible (ou caché) après un clic de l'utilisateur. L'utilisation de modificateurs est facultative .


# Comment ça marche ?

Pour uttiliser la méthodhologie *BEM* il suffit de suivre sa *convention de nommage* .
En *BEM*, toutes les classes CSS sans exception commencent  par le nom du bloc. Par exemple pour le menu : *.menu* .
Si on souhaite ajouter  un élément item dans notre bloc *.menu* , on va le nommer *.menu__item.* On sépare le bloc de l'élément par deux underscores.

Le code HTML ressemblerait donc à ça :

<div class="menu
">
<div class="menu__item
">Page 1</div>
</div>

ce qui rend la lecture et la compréhenson  du code  facile, ici *.menu__item* est un élément de *.menu* .


Concernant le modificateur, on sépare le bloc ou l'élément par deux tirets *.bloc__element--modificateur* :

<div class="menu">
<div class="menu__item">Page 1</div>
<div class="menu__item  menu__item--is-open
">Page 2</div>
<div class="menu__item">Page 3</div>
</div>



Cette façon d'écrire et une norme c'est donc une recommandation, vous êtes libre d'utiliser un underscore plutôt que deux, ou faire du camel case. Il faut simplement respecter une hiérarchie et rendre le code aussi lisible que possible.

#Pourquoi l'uttiliser ?


 BEM rend le développement d'interface facile et rapide, même avec une interface utilisateur complexe, et permet de réutiliser le code existant sans copier-coller,car comme dit plus haut c'​​est une approche du développement Web basée sur des composants. L'idée est de diviser l'interface utilisateur en blocs indépendants.

Les avantages :

**C'est modulaire**
Les styles de bloc ne dépendent jamais d'autres éléments d'une page,on ne rencontre donc jamais de problèmes de cascade .
on obtient également la possibilité de transférer des blocs de nos projets terminés vers de nouveaux. 

**Ça rend Réutilisable**
La composition de blocs indépendants de différentes manières, et leur réutilisation intelligente, réduisent la quantité de code CSS que l'on devra gérer.

Avec un ensemble de directives de style en place, on peut créer une bibliothèque de blocs, ce qui rend notre CSS super efficace. 

**Ça structure**
La méthodologie *BEM* donne à notre code CSS une structure solide qui reste simple et facile à comprendre.




voila en éspérant vous avoir éclairé sur le sujet a bientot pour plus de pécision sur le sujet








                                                                                    Bafodé,Richard,Anais,Mikael et Benoit 

   
