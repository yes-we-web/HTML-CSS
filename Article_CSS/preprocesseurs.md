# LES PREPROCESSEURS.

## Définitions.

C'est un outil ou programme permettant de générer dynamiquement des fichiers CSS. L'objectif est d'améliorer le CSS, en apportant au développeur plus de fléxibilité.

Il intervient avant le traitement du fichier par le navigateur.

## les + et les -.

Les préprocesseurs ne sont pas nécessaires mais ils permettent de facilité et gagner du temps pour le développeur.


Par exemple, lorsque tu cherches à rendre ta mise en forme compatibilible entre tous les navigateurs même les anciens natigateurs. Ils sont utiles pour ton confort de développeur, car ils permettent une meilleure organisation et productivité. Ils sont aussi un outil pour la maintenance du code lorsque le code CSS est très long.

 En d'autres termes, les preprocesseurs :
 * regroupent les codes en évitant les répétitions.
 * ils corrigent certains codes.
 * ils permettent de modifier son code CSS plus simplement...


L'extension ou "plugin" ou "add-on" permet d'ajouter des fonctionnalités aux préprocesseurs.
On peut tout à fait utliser plusieurs préprocesseurs pour un même travail.


## les différents préprocesseurs.


### PostCSS
C'est le préprocesseur le plus personnalisable selon l'envie de son utilisateur. C'est le couteau suisses.

### Less
En concurrence avec SASS, il a perdu la guerre de la popularité.

![fight](https://blog.rapid7.com/content/images/le-img/2014/10/which-css-preprocessor-should-you-choose.png)

### SASS
le plus utilisé et le plus populaire.

![sass](https://zestedesavoir.com/media/galleries/848/caf928bf-ca8a-4170-b9c2-501a52c9e65c.png)


On travaille depuis l'éditeur de commande.
Pour SASS on crée des dossiers et des fichiers (extension .scss) en supplément du index.html et style.css

### Stylus - le petit nouveau.
Ceux qui utilisent JavaScript (JS) l'apprécieront car il est programmé en JS.



## SASS en détail.


Connecte-toi sur https://www.sassmeister.com

![SASSWeb](https://github.com/yes-we-web/HTML-CSS/blob/master/Article_CSS/images/Screenshot%20from%202019-08-19%2015-50-46.png?raw=true)


Rendre ton code sur SASS en "input".

Le préprocesseur SASS traduira ton code (à revoir)


### installer SASS.

Il faut l'installer depuis le terminal.

sudo npm install -g sass

attention !!! Il faut à jour node et npm. 


### Les principales fonctionalités de SASS.

* l'imbrication : évite de répéter des "class" et/ou "balise" de nombreuses fois dans le CSS.
Attention : ne pas utiliser massivement au risque de rendre moins lisible le CSS.

![SASSimbrication](https://github.com/yes-we-web/HTML-CSS/blob/master/Article_CSS/images/SASSImbrication.jpg?raw=true)


* l'héritage : un petit raccourci qu'on appelle "@extend" permet d'étendre des règles CSS d'une "class" à une autre. Pratique!! Mais attention de ne pas en abuser pour ne pas risquer de perdre le nord.

Il y a aussi le % permet de créer de "fausse" "class" qui ne seront pas visible dans le CSS, mais qu'on pourra appeler si besoin grâce à "extend".

(Rajouter un exemple)



### Pour plus d'information.

https://sass-lang.com/guide

https://sass-lang.com/documentation

https://www.grafikart.fr/formations/sass-preprocesseur



J'espère que ça vous a plu. 

L'équipe HTML-CSS.



