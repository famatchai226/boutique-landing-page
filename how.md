# Boutique Landing Page

## Description

Page vitrine centrale ("boutique") qui présente les 6 autres landing pages comme des produits. Chaque carte produit dispose de deux actions :
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
│   ├── products/       # Visuels des 6 produits
│   │   ├── baltazar.jpg
│   │   ├── pastor.png
│   │   ├── kera.jpg
│   │   ├── bd.jpg
│   │   ├── secrets369.jpg
│   │   └── gotelegram.jpg
│   └── moyens-paiement.png
├── .gitignore
└── how.md              # This file
```

## Produits & liens

| Produit | Landing (URL Cloudflare) | Prix | Checkout MyMaketou |
|---|---|---|---|
| Pack Baltazar | `https://balta.famatchai226.workers.dev/` | 5 500 FCFA | `baltazar.mymaketou.shop/products/veux-tu-1385-video-289-photo-260-bd-video-baltazar-et-du-petit-baltazar-inclu/checkout` |
| Influenceuse Ivoirienne | `https://pastor.famatchai226.workers.dev/` | 5 500 FCFA | `baltazar.mymaketou.shop/products/acces-prive-a-des-videos-dune-influenceuse-ivoirienne-7/checkout` |
| Pack KERA | `https://kera.famatchai226.workers.dev/` | 5 500 FCFA | `baltazar.mymaketou.shop/products/acces-prive-et-discret-des-videos-dune-influenceuse/checkout` |
| Pack +14 838 BD | `https://bd.famatchai226.workers.dev/` | 13 000 FCFA | `baltazar.mymaketou.shop/products/veut-tu-14838-pdf-bd-hentai-pour-homme-mature-/checkout` |
| 369 Secrets | `https://369-secrets.famatchai226.workers.dev/` | 19 000 FCFA | `mr-livre.mymaketou.shop/products/offre-speciale-pdfaudio/checkout` |
| Guide Télégram | `https://gotelegram.famatchai226.workers.dev/` | 5 500 FCFA | `baltazar.mymaketou.shop/en/products/comment-cree-ou-recuperer-son-compte-telegram-facilement-depuis-chez-vous/checkout` |

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
2. **Hero** — Badge uniquement (titre, description et bouton retirés)
3. **Catalogue** — Grille de 6 produits + badges de confiance (juste après les produits)
4. **How it works** — 3 steps
5. **Payment** — Payment methods image
6. **FAQ** — Accordion-style questions
7. **CTA final** — Promo banner with button
8. **Footer** — Contact info
9. **Float bar** — Sticky bottom bar with promo