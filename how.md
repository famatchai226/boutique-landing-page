sf# Boutique Landing Page

## Description

Page vitrine centrale ("boutique") qui présente les 6 autres landing pages comme des produits. Chaque carte produit dispose de deux actions :
- **Voir la page** — lien relatif vers la landing page dédiée.
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

| Produit | Landing | Prix | Checkout MyMaketou |
|---|---|---|---|
| Pack Baltazar | `../balta-landing-page/index.html` | 5 500 FCFA | `baltazar.mymaketou.shop/products/veux-tu-1385-video-289-photo-260-bd-video-baltazar-et-du-petit-baltazar-inclu/checkout` |
| Influenceuse Ivoirienne | `../pastor-landing-page/index.html` | 5 500 FCFA | `baltazar.mymaketou.shop/products/acces-prive-a-des-videos-dune-influenceuse-ivoirienne-7/checkout` |
| Pack KERA | `../kera-landing-page/index.html` | 5 500 FCFA | `baltazar.mymaketou.shop/products/acces-prive-et-discret-des-videos-dune-influenceuse/checkout` |
| Pack +14 838 BD | `../bd-landing-page/index.html` | 13 000 FCFA | `baltazar.mymaketou.shop/products/veut-tu-14838-pdf-bd-hentai-pour-homme-mature-/checkout` |
| 369 Secrets | `../369-secrets-landing-page/index.html` | 19 000 FCFA | `mr-livre.mymaketou.shop/products/offre-speciale-pdfaudio/checkout` |
| Guide Télégram | `../gotelegram-landing-page/index.html` | 5 500 FCFA | `baltazar.mymaketou.shop/en/products/comment-cree-ou-recuperer-son-compte-telegram-facilement-depuis-chez-vous/checkout` |

## How to use

1. Open `index.html` in a browser.
2. The page auto-detects the browser language (French or English).
3. Click the language toggle button (FR/EN) to switch manually.

## Customization

- **Text content**: Edit `locales/fr.json` and `locales/en.json`.
- **Product links**: Update the `href` of the "Voir la page" and "Acheter" buttons in `index.html`.
- **Assets**: Replace images in `assets/products/` with your own.
- **Email**: Update the `mailto:` link in the footer.

## Sections

1. **Navbar** — Logo + language toggle + CTA button
2. **Hero** — Headline, description, trust badges
3. **Catalogue** — Grid of 6 product cards (visual, badge, price, Voir la page / Acheter)
4. **How it works** — 3 steps
5. **Payment** — Payment methods image
6. **FAQ** — Accordion-style questions
7. **CTA final** — Promo banner with button
8. **Footer** — Contact info
9. **Float bar** — Sticky bottom bar with promo