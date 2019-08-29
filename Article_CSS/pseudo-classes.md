# Pseudo classes CSS

Salut à tous, 

De retour avec le sourire, nous espérons que vous aussi ! 
Aujourd'hui à l'ordre du jour, nous parlerons des PSEUDO-CLASSES en CSS.  
Je vous vois déjà venir mais kezako ? Je ne pige pas... Pas de panique. 

Histoire de donner une définition type-top : les *speudos classes*, permettent de *changer le style d'un élément HTML* selon son état et cela de manière dynamique. 
Par exemple on peut mettre un paragraphe en gras et lorsque l'utilisateur passe son curseur en cliquant, le lien devient bleu pour spécifier qu'on est allé dessus. 
Vous voyez ? Non ? Mais si je suis sûre... Visuellement cela devrait vous parler : 


![Visuel lien pseudo code fichier index](https://www.pierre-giraud.com/html-css/cours-complet/imgs/elements-html-modifies-pseudo-classes-css.png)




Le code HTML : 



![HTML code pseudo-classe link](https://www.pierre-giraud.com/html-css/cours-complet/imgs/pseudo-classes-css.png)

![Code CSS pseudo classe link](https://www.pierre-giraud.com/html-css/cours-complet/imgs/utilisation-pseudo-classes-css.png)

Ce que l'on peut dire c'est qu'il existe plusieurs types de pseudo-classes CSS  : 

- **:link, :visited, :hover et :active**
--> Celles-ci ont un lien direct avec le HTML 
- **:first-child** et **:last-child**
- **:nth-child()**

Première observation : toutes les pseudos-classes commencent par le symbole *":"*
La première catégorie de pseudo-classes est généralement à utiliser en mode package dans l'ordre suivant : **:link, :visited, :hover et :active**

- : **link** ==> permet de styliser un lien avant que celui-ci ne soit utilisé 
Ex :

`a:link {
    color : bleu; 
    text-decoration: underline;
    }`

- **:visited** : permet de styliser un lien une fois qu'il a été visité. 

Ex: 

`a:visited {
    color : pink;
    }`

**__Remarque__** : A cause des problèmes de faille, il vaut mieux éviter de se servir de cette fonctionnalité.
- :hover : va nous permettre de changer l’aspect d’un élément lorsque vos visiteurs poseront leur curseur dessus

Ex : 

`h1:hover {
    text-decoration-color: orangered; 
    }`

-  **:active** : modification d'un élément quand on clique. 

La seconde catégorie de pseudo classe concerne **:first-child** et **:last-child**
Souvenez vous, le CSS fonctionne en cascade, il y a donc une corrélation entre grands-parents, parents, enfants. 
La pseudo classe :first-child permet donc simplement de sélectionner le premier élément enfant et la pseudo-classe :last-child la dernière.

Exemple : 

![code pseudo-classes :first-child and :last-child](https://www.pierre-giraud.com/html-css/cours-complet/imgs/first-child-last-child-css.png)

    `p:first-child {
        color : orange; 
    }
    
    p:last-child {
        color : green; 
    }`


![résultat code speudo-classes :first-child and :last-child](https://www.pierre-giraud.com/html-css/cours-complet/imgs/element-p-modifie-pseudo-classe-css.png)

La troisième catégorie concerne **:nth-child ()**. 
Elle permet de cibler plusieurs éléments d'un HTML en fonction de leur ordre dans la source et selon les critères définient. Pour cela on donnera un nombre ou un mot dans les parenthèses. 

Exemple : 
Le code HTML :

![code html pseudo-classes :nth-child](https://www.pierre-giraud.com/html-css/cours-complet/imgs/presentation-pseudo-classe-css-nth-child.png)

Le code CSS : 

![code css pseudo-classes :nth-child](https://www.pierre-giraud.com/html-css/cours-complet/imgs/utilisation-pseudo-classe-css-nth-child.png)

Résultat : 

![résultat pseudo-classes :nth-child](https://www.pierre-giraud.com/html-css/cours-complet/imgs/demonstration-pseudo-classe-css-nth-child.png)



Si vous souhaitez en savoir plus, il existe un nombre non-exhaustif de pseudo-classes. Pour les grands curieux que vous êtes voici une bonne source : [index standard of speudo-classes](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes#Index_of_standard_pseudo-classes.org)

Le team vous remercie ! :hand: 


Bafodé, Richard, Mickael, Benoît, Anaïs.
