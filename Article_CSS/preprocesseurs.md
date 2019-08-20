# LES PREPROCESSEURS.

## Définitions.

Ceux sont des outils ou programmes permettant de générer dynamiquement des fichiers CSS. L'objectif est d'améliorer le CSS, en apportant au développeur plus de fléxibilité, d'organisation et de confort.

Ils interviennent avant le traitement du fichier par le navigateur.

Les préprocesseurs ne sont pas indispensables mais utiles.

 En d'autres termes, que peuvent-ils faire ?

 * regrouper les codes en évitant les répétitions,
 * corriger certains codes,
 * modifier son code CSS plus simplemen,
 * effectuer de la maintenance,
 * aider à rendre compatibles ton CSS sur tous les navigateurs, même les plus anciens,
 * permettre de mieux gérer le responsive et les medias queries,
 * Entre autres ...


## les différents préprocesseurs.

Et oui il y en a plusieurs. Quels sont-ils ?

![UseOfPreprocessor2017](https://www.keycdn.com/img/blog/sass-vs-less-poll.webp)
Source: 2015 Survey from ashleynolan.co.uk Disclaimer: these are just responses from a small portion of developers.

### PostCSS
C'est le préprocesseur le plus personnalisable selon l'envie de son utilisateur. C'est le couteau suisses.

### Less
En concurrence avec SASS, il a perdu la guerre de la popularité.
il est programmé en JavaScript.

![fight](https://blog.rapid7.com/content/images/le-img/2014/10/which-css-preprocessor-should-you-choose.png)

### SASS
le plus utilisé et le plus populaire.
Il est programmé en Ruby.

![sass](https://zestedesavoir.com/media/galleries/848/caf928bf-ca8a-4170-b9c2-501a52c9e65c.png)


### Stylus - le petit nouveau.
Ceux qui utilisent JavaScript (JS) l'apprécieront car il est programmé en JS.



## SASS en détail.

Vous allez découvrir le merveilleux monde de SASS. Let's go!!

### installer SASS.

Il faut d'abord installer  SASS depuis le terminal.


```
sudo npm install -g sass
```

attention !!! Il faut mettre à jour node et npm.


### Les principales fonctionalités de SASS.

Il y en a beaucoup trop pour vous faire la liste exhaustive. Alors voyons les intéressantes à notre niveau.


* _**l'imbrication**_: il évite de répéter des "class" et/ou "balise" de nombreuses fois dans le SCSS.

![SASSimbrication](https://github.com/yes-we-web/HTML-CSS/blob/master/Article_CSS/images/SASSImbrication.jpg?raw=true)

Attention! Ne pas utiliser massivement car le risque  est de rendre moins lisible le CSS.


* _**l'héritage**_ : un petit raccourci qu'on appelle "@extend" permet d'étendre des règles CSS d'une "class" à une autre. Pratique!! Mais attention de ne pas en abuser pour ne pas risquer de perdre le nord.

(mettre un exemple)

Il y a aussi le "%" qui permet de créer une "class" qui ne sera pas prise en compte dans le CSS, sauf si tu décides, en tant que programmeur de l'appliquer. Alors pour l'appeler tu auras besoin de "@extend".

(mettre un exemple)


* _**Les variables**_ : Considérez les variables comme un moyen de stocker les informations que vous souhaitez réutiliser dans votre feuille de style. Vous pouvez stocker des éléments tels que les couleurs, les polices ou toute autre valeur CSS que vous pensez vouloir réutiliser. Sass utilise le symbole $ pour transformer quelque chose en une variable. 

On pourrait probablement le comparer à un alias pour le CSS.

Voici un exemple:



$ suivi du nom de la variable. C'est comme les alias.
$padding, $primary
gérer le responsive

* Fonctions :
darken/lighten - contast de la couleur
rgba - changer un couleur en rgba
il y a beaucoup de fonctions disponibles.


possibilité d'utilisé +, - , x 


### Les partials

Il est préférable de faire des dossiers et fichiers différents pour scss et importer dans un scss principal en indiquant :
```md
@import 'NomFichier';
```

Attention, pour les fichiers partials .scss il faut mettre un "_" au début du nom de fichier.



### Pour plus d'information.

https://sass-lang.com/guide

https://sass-lang.com/documentation

https://www.grafikart.fr/formations/sass-preprocesseur



J'espère que ça vous a plu. 

L'équipe HTML-CSS.



variables, nesting, mixins, inheritance and other nifty goodies that make writing CSS fun again.


L'extension ou "plugin" ou "add-on" permet d'ajouter des fonctionnalités aux préprocesseurs.


Rendre ton code sur SASS en "input".

Le préprocesseur SASS traduira ton code (à revoir)


On travaille depuis l'éditeur de commande.
Pour SASS on crée des dossiers et des fichiers (extension .scss) en supplément du index.html et style.css



