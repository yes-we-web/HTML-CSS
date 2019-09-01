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
