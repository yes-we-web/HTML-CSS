# 7-1 SASS Architecture

> Le modèle **7-1** est un moyen populaire et effectivement modulaire de structurer les projets Sass . Si votre stage ou votre lieu de travail éventuel utilise Sass, il est fort probable qu'ils utilisent certaines variantes de ce type d'architecture. Veillons donc à vous familiariser avec ce sujet avant de continuer!

## Exemples :

sass/
|
|– abstracts/
|   |– _variables.scss    # Sass Variables
|   |– _mixins.scss       # Sass Mixins
|
|– vendors/
|   |– _bootstrap.scss    # Bootstrap
|
|– base/
|   |– _reset.scss        # Reset/normalize
|   |– _typography.scss   # Typography rules
|
|– layout/
|   |– _navigation.scss   # Navigation
|   |– _grid.scss         # Grid system
|   |– _header.scss       # Header
|   |– _footer.scss       # Footer
|   |– _sidebar.scss      # Sidebar
|   |– _forms.scss        # Forms
|
|– components/
|   |– _buttons.scss      # Buttons
|   |– _carousel.scss     # Carousel
|   |– _cover.scss        # Cover
|   |– _dropdown.scss     # Dropdown
|
|– pages/
|   |– _home.scss         # Home specific styles
|   |– _contact.scss      # Contact specific styles
|
|– themes/
|   |– _theme.scss        # Default theme
|   |– _admin.scss        # Admin theme
|
 – main.scss              # Main Sass input file


1. Abstracts :

> **Abstracts** ne contient pas de styles , mais juste des mécanismes Sass permettant de définir des styles dans d’autres répertoires (parfois appelés "assistants"). Cela inclut des choses comme les variables globales, les fonctions et les mixins. Chacune de ces catégories doit être placée dans son propre fichier partiel, nommé comme il convient, comme indiqué ci-dessus.

2. Vendors :

> **Vendors** contient toutes les feuilles de style tierces utilisées par un projet. Par exemple, si nous voulions utiliser Bootstrap avec notre propre Sass personnalisé dans un projet, nous téléchargerions la feuille de style Bootstrap et la placerions ici.

3. Base :

> **Base** contient un passe-partout utilisé tout au long de la nuit. Cela inclut les styles de typographie applicables à l’ensemble du projet et les feuilles de style qui réinitialisent ou normalisent universellement les CSS par défaut.

4. Layout :

> **Layout** contient des styles pour différents aspects de la structure du site (pensez aux zones telles que les barres de navigation, les en-têtes, les pieds de page, etc.).

5. Components :

> **Components** c'est comme des "mini" mises en page. Les styles de petites pièces réutilisables du site doivent résider ici (pensez aux boutons, aux formulaires, aux images de profil, etc.)

6. Pages :

> **pages** est l'endroit où résident les styles spécifiques à la page. Par exemple, si un projet contenait plusieurs règles de style qui ne sont jamais utilisées que dans la page "Contactez-nous" , ils vivraient ici dans unfichier _contact.scss , comme indiqué ci-dessus.

7. Themes : 

> **Themes** est utilisé lorsqu'un site comporte plusieurs thèmes. Par exemple, l'exemple de projet ci-dessus inclut à la fois les thèmes admin et les thèmes par défaut. Nous pouvons donc supposer que cet exemple de site a un style totalement différent pour les administrateurs connectés. Peut-être pour mieux présenter et adapter les fonctionnalités supplémentaires d'un administrateur. Certains sites Web proposent également un «mode nuit», où l’arrière-plan du site est plus sombre, avec un texte de couleur plus claire pour une lecture plus facile dans des environnements peu éclairés. Une option comme celle-ci serait également représentée dans son propre fichier de thème.


## Import :

> Tous les fichiers de tous ces sous-répertoires sont ensuite importés dans le fichier d'entrée main.css , dans l'ordre indiqué ci-dessus, comme suit :

`- @import 'abstracts/variables';
- @import 'abstracts/mixins';

- @import 'vendors/bootstrap';

- @import 'base/reset';
- @import 'base/typography';

- @import 'layout/navigation';
- @import 'layout/grid';
- @import 'layout/header';
- @import 'layout/footer';
- @import 'layout/sidebar';
- @import 'layout/forms';

- @import 'components/buttons';
- @import 'components/carousel';
- @import 'components/cover';
- @import 'components/dropdown';

- @import 'pages/home';
- @import 'pages/contact';

- @import 'themes/theme';
- @import 'themes/admin';`

> Mais notez **qu'il n'y a pas de styles définis directement dans le fichier d'entrée main.scss** . Dans l'architecture 7-1, tous les styles vivent dans un partiel nommé de manière appropriée et sont simplement importés dans le fichier d'entrée.
