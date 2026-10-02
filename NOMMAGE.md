# Convention de nommage

Méthode : BEM (`bloc__element--modificateur`) sur une architecture SMACSS.
Les noms reprennent ceux de la maquette Figma (Résonances).

## Préfixes

| Catégorie | Préfixe | Exemples |
|-----------|---------|----------|
| Mise en page (layout) | `l-` | `l-header`, `l-footer`, `l-grid` |
| État | `is-` | `is-active`, `is-open`, `is-error`, `is-focused` |
| Thème (couleur de scène) | `theme-` | `theme-lake`, `theme-forest`, `theme-kiosk` |
| Module | aucun | `button`, `card` |

## Pages de la maquette

Accueil (01), Programme (02), Fiche artiste (03), Billetterie (04), Infos pratiques (05).

## Composants (modules)

| Bloc | Éléments | Pages | Variantes observées |
|------|----------|-------|---------------------|
| `button` | | toutes | `--primary`, `--secondary`, `--outline`, `--ghost-light` (fond sombre) ; tailles petit / moyen / grand ; avec icône, icône seule ; survol, focus clavier, désactivé |
| `badge` | | Accueil, Programme, Fiche artiste | `--lake`, `--forest`, `--kiosk` ; statuts nouveau / dernières places / complet ; petit / grand |
| `card` | `__media`, `__title`, `__meta`, `__link` | Accueil, Programme, Fiche artiste | `--headliner`, `--compact`, `--horizontal`, sans image ; thèmes `theme-*` |
| `field` | `__label`, `__help`, `__error` | Billetterie | normal, `is-focused`, `is-error`, désactivé ; champ texte, liste déroulante |
| `checkbox` | | Billetterie | cochée, non cochée |
| `filter` | `__button` | Programme | `__button.is-active` |
| `faq` | `__item` | Infos pratiques | `__item.is-open` |
| `pass` | `__ribbon` | Billetterie | `--featured` |
| `scene-banner` | | Accueil | `theme-lake`, `theme-forest`, `theme-kiosk` |
| `info-block` | | Infos pratiques | numéro 1, 2, 3 |
| `contact-band` | | Infos pratiques | |
| `stat` | | Accueil | |
| `hero` | `__media`, `__overlay` | Accueil | |
| `page-title` | | Programme, Billetterie, Infos pratiques | |
| `artist` | `__media`, `__bio`, `__infos` | Fiche artiste | `main.theme-*` |
| `booking-form` | | Billetterie | |
| `nav` | | toutes (en-tête) | lien actif `is-active` |
| `logo` | | toutes (en-tête) | |

## Mise en page (layout)

| Bloc | Rôle |
|------|------|
| `l-header` | En-tête (logo, navigation, boutons) |
| `l-footer` | Pied de page |
| `l-grid` | Grille de cartes (programme par jour, têtes d'affiche, formules) |

## Notes

- Le bouton de bascule du mode sombre est nommé `theme-toggle` dans Figma : c'est un `button` (modifieur `--outline`), pas un thème de scène.
- Ce fichier est mis à jour si un nom change pendant le projet.
