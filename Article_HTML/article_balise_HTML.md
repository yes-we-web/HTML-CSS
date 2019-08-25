# Les balises HTML

Chaque fichier texte HTML contiennent des balises (ou tag en anglais). Les balises en question doivent être utilisées d'une certaine façon afin de décrire correctement la structure de notre page.

Les balises indiquent au navigateur comment il doit séparer notre page. Certaines balises permettent quant à elles d'intégrer différents médias comme des images, des vidéos ou des musiques parmi le reste de notre contenu.

Le navigateur n'affiche pas les balises telles quelles. Lorsqu'un utilisateur visite une page web, son navigateur analyse (ou parse en anglais) le document et l'interprète afin d'afficher la page web correctement.

Par exemple, si le document contient une balise ```<img>```, le navigateur chargera l'image associée et affichera l'image à la place de la balise HTML.

## Fonctionnement de base

Les balises HTML respectent une syntaxe simple et stricte :

* Un chevron ouvrant (<)
* Le nom de la balise
* Des attributs (optionnels). Un espace, suivi du nom de l'attribut, d'un signe égal (=) et d'une valeur entre doubles quotes ("").
* Un chevron fermant (>)

Voici quelques exemples :

* ```<article>```
* ```<link rel="stylesheet" href="EmplacementDeMonFichierCSS">```
* ```<img src="monImage.png" alt="">```

Généralement, les balises fonctionnent par paires.
La première balise est la balise ouvrante et la seconde est la balise fermante. Une balise fermante doit avoir le même nom que la balise ouvrante correspondant avec une barre oblique au début du nom.

Exemple, si ```<body>``` est une balise ouvrante, ```</body>``` sera la balise fermante correspondante.

![Image démonstrative d'une balise par MDN](https://mdn.mozillademos.org/files/8573/anatomy-of-an-html-element.png)

## Les balises les plus utilisées

| Balise | Description |
| :----: | :---------: |
| ```<header>``` | Représente un groupe de contenu introductif ou de contenu aidant à la navigation.|
| ```<main>``` | "LE" contenu important d’une page HTML, cette balise ne peut donc être utilisée qu’une fois par page |
| ```<footer>``` | Représente le pied de page ou de section, il contient habituellement des informations sur l'auteur de la section, les données relatives au droit d'auteur (copyright) ou les liens vers d'autres documents en relation. |
| ```<h1>, <h2>, <h3>, <h4>, <h5>, <h6>``` | Utilisés pour la hiérarchisation des titres. |
| ```<p>``` | Définis un paragraphe contenant une ou plusieurs phrases. |
| ```<a>``` | Utilisée pour les hyperliens. |
| ```<img>``` | Permet d'insérer une image. |
| ```<ul>, <ol> et <li>``` | Ces balises sont utilisées pour créer des listes. ```<ul>``` permet de définir une liste non-ordonnée et ```<ol>``` de définir une liste ordonnée. ```<li>``` permet de définir une élément de la liste. |
| ```<aside>``` | Une partie d'un document dont le contenu n'a qu'un rapport indirect avec le contenu principal du document. |
| ```<article>``` | Utilisé pour du contenu ayant son propre sens indépendamment du reste des autres éléments de la page, ce contenu est distribuable et réutilisable. |
| ```<section>``` | Utilisée pour regrouper des éléments différents, mais partageant la même thématique. |
| ```<nav>``` | Destinée à la navigation dans un document (avec des menus, des tables des matières, des index, etc.). |

### Source et liens utiles

* [Liste complète des balises](https://jaetheme.com/balises-html5/)
* [Article sur les balises HTML et leur rôles](https://developer.mozilla.org/fr/docs/Apprendre/HTML/Balises_HTML)
