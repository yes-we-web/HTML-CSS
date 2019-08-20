# LES PREPROCESSEURS.

## Définitions.

Ceux sont des outils ou programmes permettant de générer dynamiquement des fichiers CSS. L'objectif est d'améliorer le CSS, en apportant au développeur plus de fléxibilité, d'organisation et de confort.

Ils interviennent avant le traitement du fichier par le navigateur.

Les préprocesseurs ne sont pas indispensables mais utiles.

 En d'autres termes, que peuvent-ils faire ?

 * regrouper les codes en évitant les répétitions,
 * corriger tes codes,
 * modifier ton code CSS plus simplement,
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


### Installer SASS.

Il faut d'abord installer  SASS depuis le terminal.

```
sudo npm install -g sass
```

attention !!! Il faut mettre à jour node et npm.


### Utiliser SASS.

Une fois Sass installé, tu peux compiler Sass en CSS à l’aide de la commande sass depuis le terminal.

tu dois indiquer à Sass le fichier à partir duquel construire et où générer le code CSS. Par exemple, exécuter à partir de votre terminal :

```
sass input.scss output.css
```
Il prend un seul fichier Sass, **input.scss** (le fichier d'entrée de la programmation avec SASS), et le compile dans **output.css** (la réponse de SASS traduit en language CSS).

Une fois que vous aurez commencé à bricoler avec Sass, votre fichier Sass prétraité sera sauvegardé et enregistré en tant que fichier CSS normal que vous pourrez utiliser sur votre site Web.


### Les principales fonctionalités de SASS.

Il y en a beaucoup trop pour vous faire la liste exhaustive. Alors voyons les plus intéressantes à notre niveau.

* _**L'--watch**_ : tu peux regarder des fichiers ou des répertoires avec l'indicateur --watch. L'indicateur de surveillance indique à Sass de surveiller les modifications apportées à tes fichiers source et de recompiler les CSS chaque fois que tu enregistres dans Sass. Si tu veux regarder ton fichier input.scss, ajoute simplement l'indicateur de surveillance à ta commande depuis le terminal, comme suit:

```
sass --watch input.scss output.css
```

Il est génial pour répérer des erreurs dans ton CSS !!!


* _**l'imbrication ou "nesting"**_: il évite de répéter des "class" et/ou "balise" de nombreuses fois dans le SCSS. L'imbrication est un avantage énorme par rapport à CSS car elle crée une hiérarchie visuelle, similaire à celle que tu as l'habitude d'utiliser avec HTML. Dans les exemples, tu peux voir à quel point il est moins nécessaire de répéter des classes ou des div étant donné qu’il s’agit maintenant d’une approche en cascade.

![SASSimbrication](https://github.com/yes-we-web/HTML-CSS/blob/master/Article_CSS/images/SASSImbrication.jpg?raw=true)

Attention! Ne pas l'utiliser massivement car le risque  est de rendre moins lisible le CSS.


* _**Les variables**_ : Avec SASS, tu as l’avantage sur les CSS classiques car tu peux utiliser des variables. Tu peux stocker des éléments tels que les couleurs, les polices de caractères ou pratiquement toutes les valeurs que tu souhaites réutiliser ultérieurement. Considére les variables comme un moyen de stocker les informations. Sass utilise le symbole $ pour transformer quelque chose en une variable. Voir l'exemple ci-dessous.

![SASSheritage](https://github.com/yes-we-web/HTML-CSS/blob/master/Article_CSS/images/variablesexampleSASS.jpg)


* _**L'héritage avec @extend**_ : Ceci est une autre fonctionnalité puissante. Il te permet de partager des propriétés d'un sélecteur à un autre.

![SASSextendSCSS](https://github.com/yes-we-web/HTML-CSS/blob/master/Article_CSS/images/extendSASS.jpg)
![SASSextendCSS](https://github.com/yes-we-web/HTML-CSS/blob/master/Article_CSS/images/extend2SASS.jpg)

Pratique!! Mais attention de ne pas en abuser pour ne pas risquer de perdre le nord.

NB : il y a aussi le "%" qui permet de créer une "class" qui ne sera pas prise en compte dans le CSS, sauf si tu décides, en tant que programmeur, de l'appliquer. Alors pour l'appeler tu auras besoin de "@extend".


* _**Les partials**_ : Le fichier CSS @import standard te permet de fractionner plusieurs fichiers. Le problème, c'est que cela crée des requêtes HTTP supplémentaires. Sass travaille un peu différemment. Au lieu de créer une autre requête HTTP, ils combinent les fichiers en une seule.

tu pourras faire des dossiers et fichiers différents pour chaque type de programmation (boutons, médiaqueries etc...) et importer dans un scss principal en indiquant :
```md
@import 'NomFichier';
```
Attention, pour les fichiers partials .scss il faut mettre un "_" au début du nom de fichier. L'underscore indique à Sass que le fichier est un fichier partiel et qu'il ne doit pas être généré dans un fichier CSS.

Les partials sont très utiles pour l'organisation du programmeur. Tu le découvriras en travaillant.


### Pour plus d'information.

https://sass-lang.com/guide

https://sass-lang.com/documentation


J'espère que ça t'a plu. 

L'équipe HTML-CSS.


