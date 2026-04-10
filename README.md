# 💊 Ouate Pharmacie BE — Landing Page Revendeurs

Landing page B2B dédiée au programme de partenariat revendeur **Ouate Le Touquet-Paris-Plage** pour les pharmacies en **Belgique** et au **Luxembourg**.

Développée et maintenue par [Nexxia Studio](https://github.com/nexxia-studio) pour **HElo Cosmetics**, distributeur officiel Ouate en Belgique et Luxembourg.

---

## 🎯 Objectif

Capturer des prospects pharmaciens qualifiés via une annonce sponsorisée (Google Ads / Meta Ads) et les transmettre automatiquement à l'équipe commerciale.

---

## ⚙️ Stack technique

| Composant | Solution |
|---|---|
| Page | HTML / CSS / JS — fichier unique |
| Hébergement | GitHub Pages |
| Formulaire | [Formspree](https://formspree.io) |
| Notification email | Formspree → info@helocosmetics.com |
| Base de données prospects | Google Sheets via Apps Script |
| Autocomplétion pharmacies | Registre AFMPS — 4 556 pharmacies agréées BE (07/04/2026) |

---

## 🗂️ Structure du repo

```
helo-ouate-pharmacie-be/
├── index.html        # Landing page complète (HTML + CSS + JS embarqués)
└── README.md         # Ce fichier
```

---

## 🔗 Intégrations

### Formspree
- Endpoint : `https://formspree.io/f/xgopjlkn`
- Projet Formspree : `Ouate Pharmacie BE`
- Destinataire : `info@helocosmetics.com`
- Objet automatique : `🟡 Nouveau prospect pharmacie — [Nom de la pharmacie]`

### Google Sheets
- Script de réception : Google Apps Script déployé en Web App
- Colonnes : Date · Heure · Région · Pharmacie · Adresse · CP · Ville · Contact · Email · Téléphone · Rôle · Rayon bébé · Message · Statut
- Région déduite automatiquement du code postal

---

## ✅ Champs du formulaire

- Pharmacie *(autocomplétion sur 4 556 officines agréées)*
- Prénom / Nom
- Email professionnel *(validation + blocage domaines jetables)*
- Téléphone *(formats BE, LU, FR uniquement)*
- Rôle dans la pharmacie
- Rayon cosmétique bébé/enfant existant
- Message libre *(optionnel)*

---

## 🌍 SEO & GEO

- Balises meta, Open Graph, Twitter Card
- Ciblage géographique `geo.region: BE`
- Schema.org JSON-LD : `ContactPage`, `Organization`, `Product`, `FAQPage`
- Langue : `fr-BE`
- Canonical : `https://pharmacie.ouate-paris.be`

---

## 🚀 Déploiement

La page est déployée via **GitHub Pages** sur la branche `main`.

URL GitHub Pages :
```
https://nexxia-studio.github.io/helo-ouate-pharmacie-be
```

Sous-domaine custom :
```
https://pharmacie.ouate-paris.be
```

### Pointer le sous-domaine (DNS)
Ajouter un enregistrement **CNAME** chez le registrar de `ouate-paris.be` :
```
pharmacie  →  nexxia-studio.github.io
```

---

## 📋 Roadmap

- [x] Formulaire HTML brandé Ouate
- [x] Autocomplétion 4 556 pharmacies AFMPS
- [x] Validation téléphone BE/LU/FR
- [x] Validation email + blocage domaines jetables
- [x] Connexion Formspree
- [x] Automation Google Sheets
- [x] SEO & GEO optimisé
- [x] Schema.org JSON-LD
- [ ] Sous-domaine `pharmacie.ouate-paris.be` actif
- [ ] Version concept stores / petite enfance

---

## 👤 Contact

**HElo Cosmetics** · Distributeur officiel Ouate — Belgique & Luxembourg
[ouate-paris.be](https://www.ouate-paris.be) · info@helocosmetics.com
