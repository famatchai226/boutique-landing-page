# Boutique Landing Page

## Description

Page vitrine centrale (« boutique ») qui présente les 7 produits du catalogue, chacun relié à sa landing page dédiée. Chaque carte produit dispose de deux actions :
- **Voir la page** — URL Cloudflare vers la landing page dédiée.
- **Acheter** — lien direct vers le checkout MyMaketou correspondant.

## Structure

```
boutique-landing-page/
├── index.html          # La boutique (catalogue)
├── i18n.js             # Internationalisation (FR/EN)
├── locales/
│   ├── fr.json         # Traductions françaises
│   └── en.json         # Traductions anglaises
├── assets/
│   ├── products/       # Visuels des 7 produits (WebP servis par index.html)
│   │   ├── baltazar.webp
│   │   ├── pastor.webp
│   │   ├── kera.webp
│   │   ├── bd.webp
│   │   ├── cecelove.webp     # film, volet 1
│   │   ├── cecelove2.webp    # film, volet 2
│   │   └── gotelegram.webp
│   └── moyens-paiement.png
├── .gitignore
└── how.md              # This file
```

## Produits & liens

**URL déployée de la boutique** : `https://boutique-landing-page.famatchai226.workers.dev/`
(c'est la cible de la carte « boutique complète » des pages CeceLove).

| Produit | Landing (URL Cloudflare) | Prix | Checkout MyMaketou |
|---|---|---|---|
| Pack Baltazar | `https://balta.famatchai226.workers.dev/` | 5 500 FCFA | `baltazar.mymaketou.shop/products/veux-tu-1385-video-289-photo-260-bd-video-baltazar-et-du-petit-baltazar-inclu/checkout` |
| Influenceuse Ivoirienne | `https://pastor.famatchai226.workers.dev/` | 5 500 FCFA | `baltazar.mymaketou.shop/products/acces-prive-a-des-videos-dune-influenceuse-ivoirienne-7/checkout` |
| Pack KERA | `https://kera.famatchai226.workers.dev/` | 5 500 FCFA | `baltazar.mymaketou.shop/products/acces-prive-et-discret-des-videos-dune-influenceuse/checkout` |
| Pack +14 838 BD | `https://bd.famatchai226.workers.dev/` | 13 000 FCFA | `baltazar.mymaketou.shop/products/veut-tu-14838-pdf-bd-hentai-pour-homme-mature-/checkout` |
| Guide Télégram | `https://gotelegram.famatchai226.workers.dev/` | 5 500 FCFA | `baltazar.mymaketou.shop/en/products/comment-cree-ou-recuperer-son-compte-telegram-facilement-depuis-chez-vous/checkout` |
| CeceLove (film, volet 1) | `https://cecelove.famatchai226.workers.dev/` | 1 500 FCFA | `baltazar.mymaketou.shop/products/veux-un-film-pour-homme-mature/checkout` |
| CeceLove 2 (film, volet 2) | `https://cecelove2.famatchai226.workers.dev/` | 3 500 FCFA | `baltazar.mymaketou.shop/products/meilleur-film-mature/checkout` |

> **369 Secrets a été retiré du catalogue** : produit jugé inapproprié pour la boutique.
> Sa landing (`https://369-secrets.famatchai226.workers.dev/`) reste en ligne, inchangée,
> mais il n'est plus vendu ni mis en avant ici (carte produit, mosaïque, traductions).
>
> Les clés i18n du catalogue restent `p1`→`p4`, `p6` (guide), `p7`/`p8` (films) :
> l'emplacement `p5`, libéré par ce retrait, n'est pas réutilisé.

## How to use

1. Open `index.html` in a browser.
2. The page auto-detects the browser language (French or English).
3. Click the language toggle button (FR/EN) to switch manually.

## 18+ Age Gate

Chaque visite affiche une popup demandant si l'utilisateur a **plus de 18 ans** :
- **Oui** → la popup se ferme et la page devient accessible.
- **Non** → message « Accès refusé » et la popup reste affichée.
Le texte est bilingue FR/EN (détection automatique de la langue).

## Git — Mise à jour sur GitHub

1. Ouvrez un terminal dans le dossier : `c:\Users\hp\Antigravity& Stitch\boutique-landing-page`
2. Préparer les fichiers : `git add .`
3. Enregistrer les changements : `git commit -m "Mise à jour : boutique"`
4. Envoyer sur GitHub : `git push origin main`

*Le déploiement (Cloudflare Pages / Workers) se lancera automatiquement après le push.*

## Customization

- **Text content**: Edit `locales/fr.json` and `locales/en.json`.
- **Product links**: Update the `href` of the "Voir la page" and "Acheter" buttons in `index.html`.
- **Assets**: Replace images in `assets/products/` with your own.
- **Email**: Update the `mailto:` link in the footer.

## Sections

1. **Navbar** — Logo + language toggle + CTA button
2. **Hero** — Badge, titre, description, CTA « Voir les offres », preuve sociale et badges de confiance
3. **Catalogue** — Grille de 7 produits + badges de confiance (juste après les produits)
4. **How it works** — 3 steps
5. **Payment** — Payment methods image
6. **FAQ** — Accordion-style questions
7. **CTA final** — Promo banner with button
8. **Footer** — Contact info
9. **Float bar** — Sticky bottom bar with promo