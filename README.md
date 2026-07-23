# Les Rencontres D2X — site

Site web des **Rencontres Professionnelles de la Piscine Publique et des Équipements Sportifs**, organisées par **D2X International** depuis 2005.

Repositionnement selon le cahier des charges (avril 2026) : passer d'une vitrine d'événement à une **machine de conversion** autour de deux parcours (Collectivités / Partenaires), avec un message central « ce n'est pas un salon, c'est un système de mise en relation ».

Univers graphique **cohérent avec le site corporate d2x.fr** (fonts Inter + Space Grotesk + Instrument Serif, palette navy / bleu `#1c75bc`, composants nav blur, stats band, CTA dark).

**Code couleur persona :** orange pastel = collectivités (`--collectivite #e08a3c`), violet pastel = entreprises/partenaires (`--partenaire #8a72c9`). L'accueil reste neutre navy/bleu ; chaque page persona a son univers coloré (header, eyebrow, accroche serif, boutons).

## Structure

- `index.html` — Accueil (orientation anti-salon + double entrée persona)
- `collectivites.html` — Tunnel collectivités (« je porte un projet »)
- `partenaires.html` — Tunnel partenaires (ROI / accès aux projets qualifiés)
- `evenement.html` — Édition 2026 (12–14 oct.) + historique
- `ressources.html` — Plateforme annuelle (portraits, guides, newsletter)
- `a-propos.html` — Histoire, équipe, presse
- `contact.html` — Formulaire qualifié multi-étapes (profil → qualification → coordonnées)
- `mentions-legales.html`
- `styles.css` — design system partagé
- `assets/` — favicons + logo D2X

## À compléter avant mise en ligne

Contenu réel déjà intégré (source : site live rencontresd2x.com) : lieu **Van der Valk Hotel Paris CDG Airport**, édition **23es (12–14 oct. 2026)**, email **rp@d2x.fr** + portable **06 79 89 58 45**, format **5 RDV de 25 min / 6 collectivités à sélectionner**, **liste réelle des partenaires 2025** (page collectivités).

Rechercher les repères `À COMPLÉTER` (classe `.todo`) restants :
- Programme détaillé jour par jour, chiffres/faits par édition
- Vrais témoignages (nom + fonction) — absents du site live, à fournir ; photos/vidéos, portraits Ressources
- Formulaires : brancher le lien Fillout (collectivités) et le circuit devis (partenaires)
- Mentions légales : forme juridique, RCS, hébergeur, politique RGPD
- Équipe : photos, noms, titres
- Image Open Graph : `assets/og/og-default.jpg` (1200×630)

## Développement local

```bash
python3 -m http.server 8000
# puis http://127.0.0.1:8000
```

## Déploiement

Site statique — servable tel quel (Cloudflare Pages, Netlify, GitHub Pages, OVH…).
Domaine cible : `rencontresd2x.com` (voir `CNAME`).
