# Nomenclature : boutique d'instruments de musique

Cette liste sert de référence pour nommer les classes. Une classe qui n'est pas ici ne doit pas apparaître sans raison.

## Règles

1. Un block a un nom simple : `header`, `products`, `product`, `footer`.
2. Un élément s'écrit `block__element` (deux underscores). Il ne sort jamais de son block.
3. Un modifier s'écrit `block--modifier` ou `block__element--modifier` (deux tirets). Il s'ajoute à la classe de base, il ne la remplace pas.
4. Pas d'élément d'élément. Le prix d'un produit est `product__price`, même s'il est rangé dans une autre boîte.
5. Dans le CSS, le modifier est écrit après la classe de base.

## Header

| Classe | Rôle |
|---|---|
| `header` | Bandeau du haut, collé à l'écran (sticky) |
| `header__logo` | Nom de la boutique |
| `header__nav` | Liste de liens de navigation |
| `header__cart` | Lien ou bouton vers le panier |

## Products

| Classe | Rôle |
|---|---|
| `products` | Conteneur de la grille (flex, flex-wrap) |
| `products__title` | Titre de la section (facultatif) |

## Product (carte)

| Classe | Rôle |
|---|---|
| `product` | Une carte produit, block autonome (flex en colonne) |
| `product__image` | Photo de l'instrument |
| `product__badge` | Pastille posée sur l'image (absolute) |
| `product__badge--new` | Variante « Nouveau » |
| `product__badge--promo` | Variante « Promo » |
| `product__brand` | Nom de la marque |
| `product__name` | Nom de l'instrument |
| `product__description` | Courte description |
| `product__prices` | Boîte qui regroupe les deux prix |
| `product__price` | Prix actuel |
| `product__price--old` | Prix barré |
| `product__button` | Bouton d'ajout au panier (collé en bas avec margin-top: auto) |

## Footer

| Classe | Rôle |
|---|---|
| `footer` | Pied de page (margin-top: auto pour rester en bas) |
| `footer__text` | Mentions ou copyright |
| `footer__links` | Liste de liens secondaires |

## Mots-clés CSS liés à la nomenclature

- Variables : `--color-main`, `--color-main-dark`, `--color-bg-block` (déclarées dans `:root`).
- États : `:hover` sur `.product__button`, avec la transition déclarée sur l'état normal.
