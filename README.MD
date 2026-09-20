
# Loptishop — Vitrine e-commerce (HTML/CSS)

Site vetrine e-commerce en HTML5 et CSS3 pur (aucun framework, aucun JavaScript). 


## Structure du projet

projet-ecommerce/
── index.html Page d'accueil
── catalogue.html Grille des 8 produits
── produit.html Fiche produit détaillée
── panier.html Panier statique + formulaire de commande
── css/
 ── style.css Feuille de style unique, partagée par les 4 pages
── images/ ── hero.jpg
│ ── produit-01.jpg … produit-08.jpg
── README.md


## Choix effectués

- **Une seule feuille de style** (`css/style.css`) chargée par les 4 pages, organisée en sections commentées : reset, variables, typographie, layout, header/nav, footer, boutons, hero, grille produits, fiche produit, formulaires, panier, responsive.
- **Header et footer identiques** sur les 4 pages (recopiés à l'identique, pas de composants en HTML pur). Le lien de navigation actif est marqué avec `aria-current="page"`, stylisé directement dans le CSS partagé — pas besoin de classe différente par page.
- **CSS Grid** (`repeat(auto-fill, minmax(220px, 1fr))`) pour la grille de produits : le nombre de colonnes s'adapte automatiquement à la largeur de l'écran, sans media query dédiée.
- **Sélecteurs taille/couleur** sur la fiche produit stylisés en boutons avec des `<input type="radio">` cachés (`opacity:0`) + `<label>` associé, y compris l'état `:checked`. Reste utilisable au clavier (label + input liés par `for`/`id`).
- **Panier statique** : 3 produits figés avec quantité, sous-total par ligne et total général cohérents (15 400 DA + 500 DA de livraison = 15 900 DA), pour donner une démonstration crédible malgré l'absence de logique réelle.
- **Formulaire de commande** avec champs groupés dans des `<fieldset>`/`<legend>`, chaque champ associé à un `<label>`.
- **Responsive** : 3 paliers (mobile / tablette / desktop) via media queries à 900px et 640px — navigation empilée verticalement, grille en une colonne, tableau du panier en liste sur mobile.
- **Accessibilité** : `alt` descriptif sur toutes les images produits, focus clavier visible (`:focus-visible`) sur tous les liens, boutons et champs, contraste vérifié entre texte et fond.

## Déroulé 

1. Arborescence + page d'accueil
2. Page catalogue + grille produits
3. Fiche produit détaillée
4. Page panier + tunnel de commande
5. Interactions et responsive design
6. Validation W3C (HTML + CSS) et finitions

| Color             | Hex                                                                |
| ----------------- | ------------------------------------------------------------------ |
| Primary Color | ![#0a192f](https://dummyimage.com/10/0a192f/white?text=+) #6B4226 |
| base Color | ![#f8f8f8](https://dummyimage.com/10/f8f8f8/white?text=+) #273023;|
| secondary Color | ![#00b48a](https://dummyimage.com/10/00b48a/white?text=+) #7C8B5A |
| base Color | ![#00d1a0](https://dummyimage.com/10/00d1a0/white?text=+) #DAD3C2 |


## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://asmaakhalfoun.com/)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/asmaa-khalfoun/)



## Author
- [@asmaaaaii](https://www.github.com/asmaaaaii)