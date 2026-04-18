# Cabinet Pr M. Bouame — Landing page

Landing page premium pour le cabinet du **Pr M. Bouame**, cardiologue et cardiorythmologue interventionnel à Blida (Algérie).

Design médical, sobre et haut de gamme, avec une signature visuelle rouge bordeaux évoquant le cœur, la précision et la confiance.

---

## Aperçu

- **Nom :** Pr M. Bouame
- **Spécialité :** Cardiologue / Cardiorythmologue interventionnel
- **Adresse :** 10 Cité Le Plan Zabana, Blida
- **Téléphones :** 07 74 91 63 09 — 05 56 89 56 09
- **Email :** bouamecabcardio9@gmail.com

---

## Structure du projet

```
.
├── index.html              # Page principale
├── 404.html                # Page d'erreur
├── css/
│   └── style.css           # Styles (thème rouge bordeaux premium)
├── js/
│   └── script.js           # Interactions (menu, FAQ, reveal)
├── assets/
│   └── img/
│       ├── logo.png
│       ├── accueil.jpg
│       ├── office.jpg
│       ├── salle-examen.jpg
│       ├── test-effort.jpg
│       └── gate.jpg
├── site.webmanifest        # Manifeste PWA léger
├── robots.txt
├── sitemap.xml
├── .gitignore
└── README.md
```

---

## Lancer en local

Pas de build nécessaire — ouvrez simplement `index.html` dans un navigateur.

Pour un rendu avec rechargement et permissions locales correctes (carte embed, etc.), servez les fichiers :

```bash
# Avec Python 3
python -m http.server 8080
# Puis ouvrez http://localhost:8080
```

Ou avec Node.js :

```bash
npx serve .
```

---

## Déploiement

Le site est 100 % statique (HTML / CSS / JS). Il peut être déployé sur n'importe quel hébergeur statique :

### Option 1 — GitHub Pages

1. Créez un nouveau dépôt GitHub (ex. `bouame-cardiology`).
2. Dans le dossier du projet :

```bash
git init
git add .
git commit -m "Initial commit — Landing page Pr Bouame"
git branch -M main
git remote add origin https://github.com/<votre-compte>/bouame-cardiology.git
git push -u origin main
```

3. Sur GitHub : **Settings → Pages → Source : Deploy from branch → Branch : main / root**.
4. Le site sera accessible à `https://<votre-compte>.github.io/bouame-cardiology/`.

### Option 2 — Netlify

- Glissez-déposez le dossier du projet sur [app.netlify.com/drop](https://app.netlify.com/drop), ou connectez votre dépôt GitHub. Aucun paramètre de build n'est requis.

### Option 3 — Vercel

- Importez le dépôt sur [vercel.com](https://vercel.com). Framework : **Other**. Output directory : laissez vide.

### Option 4 — Hébergement classique (OVH, Hostinger, cPanel, etc.)

- Connectez-vous en FTP / SFTP et uploadez l'intégralité du contenu du projet dans le dossier `public_html/` (ou `www/`). Vérifiez que `index.html` se trouve à la racine.

---

## Personnalisation rapide

- **Couleurs** : modifiables dans `css/style.css` via les variables CSS au début (`:root`).
- **Contenu textuel** : directement dans `index.html`.
- **Images** : remplacez les fichiers dans `assets/img/` en gardant les mêmes noms.
- **Logo / favicon** : remplacez `assets/img/logo.png`.

---

## Accessibilité & SEO

- Hiérarchie `H1 / H2 / H3` propre.
- Attributs `alt` sur toutes les images pertinentes.
- `aria-label` et `aria-expanded` sur les éléments interactifs.
- Balises `meta` description, Open Graph et Schema.org (Physician) incluses.
- `prefers-reduced-motion` respecté.

---

## Avertissement

Les informations présentées sur ce site ont une vocation **informative** et ne remplacent en aucun cas une consultation médicale. En cas d'urgence vitale, contactez immédiatement les services d'urgence.

---

© Cabinet du Pr M. Bouame — Tous droits réservés.
