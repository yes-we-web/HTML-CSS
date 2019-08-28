# Carrousel responsif

Comment réaliser un carrousel d’images de largeur fixe en CSS :

On peut réaliser un carrousel contenant autant d’images que vous le souhaitez.
La seule condition est que toutes les images doivent avoir la même taille.

out d’abord nous avons besoin de rendre l’élément carrousel responsif. Pour cela, nous commençons avec le HTML suivant :

//HTML
<div id="slider">
  <figure>
    <img src="austin-fireworks.jpg" alt="">
    <img src="taj-mahal.jpg" alt="">
    <img src="ibiza.jpg" alt="">
    <img src="ankor-wat.jpg" alt="">
    <img src="austin-fireworks.jpg" alt="">
  </figure>
</div>

Remarquez : la même image est placée au début et à la fin de la bande, pour que l’animation fait une boucle.

Nous devons déterminer une largeur de nos images en % de préférence pour que cela soit responsive et une largeur maximum (max-width);

exemple : 
//CSS
div#slider { width: 80%; max-width: 1000px; } 

la largeur de l’élément figure est un pourcentage, qui est un multiple de la div qui le contient. Si la bande d’images contient cinq images, et que notre div n’en montre qu’une, la figure est 5x plus large, c’est à dire 500% de largeur de la div container :

/CSS
div#slider figure {
  position: relative; 
  width: 500%;
  margin: 0;
  padding: 0;
  font-size: 0;
}

Explication:
La font-size: 0, pour réduire l'espace entre les images et autour. Position: relative permet à la figure d’être déplacée facilement pendant l’animation.

Ensuite répartisons les images de manière régulière à l’intérieur de la bande. Le calcul est très simple : Si nous l’élément de la figure fait 100% de large, chaque image doit prendre 1/5 de l’espace horizontal : 100% / 5 = 20%.

La déclaration CSS suivante :

//CSS
div#slider figure img { width: 20%; height: auto }

puis nous cachons ce qui dépasse (overflow) de la div :

//CSS
div#slider { width: 80%; max-width: 1000px; overflow: hidden }.

Maintenant nous allons nous occupé de l'animation.

Il nous faut déplacer l'image de droite à gauche. Si on considère que la div container fait 100% de large, chaque mouvement de l'image vers la gauche sera mesuré en incréments de cette distance :

//CSS
@keyframes slidy {
  0% { left: 0%; }
  20% { left: 0%; }
  25% { left: -100%; }
  45% { left: -100%; }
  50% { left: -200%; }
  70% { left: -200%; }
  75% { left: -300%; }
  95% { left: -300%; }
  100% { left: -400%; }
}

Chaque image sera affichée dans la div pour 20% de la durée totale de l’animation, le temps de déplacement étant de 5%.

Il ne nous reste plus qu’à appeler notre animation pour que les choses commencent (le code est indiqué ici sans préfixes constructeurs, pour la simplicité, mais il ne faudra pas les oublier, vous pouvez utiliser Autoprefixer pour cela).

//CSS
div#slider figure {
  position: relative;
  width: 500%;
  margin: 0;
  padding: 0;
  font-size: 0;
  left: 0;
  **animation: 30s slidy infinite;**
}

Maintenant a vous de joué!

petit info :  une solution simple et rapide, CSSslidy est un petit JavaScript qui auto-génère des keyframes d’animation CSS3 pour tout type d'image.