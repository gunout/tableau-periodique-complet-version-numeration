<div align="center">

# 🌌 Tableau Périodique Complet
### Version Numérotation Alphabétique

**Une réinterprétation interactive des 118 éléments chimiques où chaque symbole est remplacé par sa numérotation alphabétique (A=1, B=2, … Z=26).**

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/fr/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/fr/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/fr/docs/Web/JavaScript)
[![License: MIT](https://img.shields.io/badge/License-MIT-002395?style=for-the-badge)](./LICENSE)

[🚀 Démo](#-utilisation) · [📖 Documentation](#-fonctionnalités) · [🐛 Signaler un bug](https://github.com/gunout/tableau-periodique-complet-version-numeration/issues)

</div>

---

## 📖 Présentation

**Tableau Périodique Complet — Version Numérotation** est une application web autonome (un seul fichier `index.html`) qui propose une **lecture alternative du tableau périodique de Mendeleïev**.

Chaque symbole chimique est converti en **code numérique alphabétique** : `H` → `8`, `He` → `8·5`, `Fe` → `6·5`, `Au` → `1·21`…

Le projet conserve néanmoins **l'intégralité des données scientifiques** : noms complets des éléments, numéros atomiques, masses, configurations électroniques, dates de découverte, découvreurs, catégories chimiques et signatures spectrales.

> 💡 **Objectif pédagogique** : offrir une nouvelle grille de lecture du tableau périodique, mêlant histoire des sciences, spectroscopie et codage alphabétique.

---

## ✨ Fonctionnalités

### 🧪 Tableau périodique interactif
- Grille complète 18 colonnes conforme à la classification standard
- Chaque case affiche : **code numérique**, **nom complet** et **numéro atomique**
- Survol animé, info-bulle contextuelle et mise en évidence des filtres actifs
- Clic sur une case → ouverture directe de la fiche détaillée

### 📅 Frise chronologique
- Nuage de points **année de découverte** × **numéro atomique**
- Code couleur par époque historique
- Légende interactive synchronisée avec les filtres

### 🏛️ Vue par époque
- 6 époques historiques : Antiquité, Moyen-Âge, Renaissance, Révolution Chimique, Ère Spectroscopique, Période Moderne
- Cartes de découverte avec bandeau spectral RGB par élément

### 🌈 Analyse spectrale
- **Par catégorie** : palettes spectrales des 10 familles chimiques
- **Par époque** : signature spectrale moyenne par période historique
- **Comparaison** : superposition jusqu'à N spectres d'émission simulés (380–780 nm)

### 🔍 Explorateur d'éléments
- Fiche détaillée : historique, propriétés atomiques, données spectrales
- Cercle chromatique RGB caractéristique
- Graphique SVG du spectre d'émission (raie principale + raies secondaires)

### 🎛️ Filtres & options
- Filtrage multi-critères par **époque** et par **catégorie**
- Options d'affichage : spectres simulés, regroupement par époque
- Navigation par sections indépendantes

---

## 🧬 Correspondance alphabétique

| Symbole | Code numérique | Nom complet | Z |
|:-------:|:--------------:|:-----------:|:-:|
| H  | `8`      | Hydrogène | 1 |
| He | `8·5`    | Hélium    | 2 |
| Li | `12·9`   | Lithium   | 3 |
| C  | `3`      | Carbone   | 6 |
| O  | `15`     | Oxygène   | 8 |
| Fe | `6·5`    | Fer       | 26 |
| Au | `1·21`   | Or        | 79 |
| U  | `21`     | Uranium   | 92 |

**Règle de conversion :** `symbole → position alphabétique (a=1, b=2, …, z=26)`, joint par un point médian `·`.

---

## 🚀 Utilisation

### Installation locale

Aucune dépendance, aucun build. Il suffit d'ouvrir le fichier :

```bash
git clone https://github.com/gunout/tableau-periodique-complet-version-numeration.git
cd tableau-periodique-complet-version-numeration

Puis ouvrez index.html dans un navigateur moderne :


# Linux / macOS
xdg-open index.html    # ou open index.html

# Windows
start index.html
```
Déploiement

L'application étant 100 % statique, elle peut être hébergée sur :

    GitHub Pages : Settings → Pages → Branch: main / root

    Netlify / Vercel / Cloudflare Pages : glisser-déposer le dépôt

    Tout serveur HTTP statique (Apache, Nginx, S3…)

🛠️ Stack technique
Couche	Technologie	Rôle
Structure	HTML5 sémantique	Contenu et accessibilité
Style	CSS3 moderne	Variables CSS, Grid, Flexbox, animations
Logique	JavaScript Vanilla (ES6+)	État, rendu dynamique, filtres
Graphiques	SVG inline	Spectres, frise chronologique
Typographie	Segoe UI / system-ui	Rendu natif, aucune dépendance externe

Aucune librairie tierce, aucun framework, aucun CDN.
📂 Structure du projet


    tableau-periodique-complet-version-numeration/
    ├── index.html      # Application complète (HTML + CSS + JS intégrés)
    ├── README.md       # Documentation du projet
    └── LICENSE         # Licence MIT

    ⚠️ Le projet est volontairement mono-fichier pour faciliter la diffusion, l'archivage et l'utilisation hors-ligne.

📊 Données embarquées

    118 éléments — numéro atomique, masse, configuration électronique, période, groupe

    Découvertes — dates et découvreurs pour chaque élément

    6 époques historiques — descriptions et palettes

    10 catégories chimiques — couleurs et codes

    Spectres simulés — longueur d'onde principale, raies secondaires, RGB

    📚 Les données sont compilées à des fins pédagogiques et peuvent être étendues en modifiant le tableau ELEMENTS dans index.html.

🎨 Aperçu des vues
Vue	Contenu
Tableau Périodique	Grille 18 colonnes, codes numériques, noms, Z
Frise Chronologique	Nuage de points année × numéro atomique
Vue par Époque	Cartes de découverte groupées par période
Analyse Spectrale	Onglets Catégorie / Époque / Comparaison
Explorateur	Fiche complète + cercle RGB + spectre SVG
🔧 Personnalisation
Modifier la conversion alphabétique

Dans index.html, la fonction symToNum() gère la conversion :
javascript

function symToNum(sym){
  return sym.split('').map(c => c.toLowerCase().charCodeAt(0) - 96).join('·');
}

Changez le séparateur '·' par '-', '' ou tout autre caractère selon vos préférences.
Ajouter ou modifier un élément

Éditez le tableau ELEMENTS (objets avec s, n, Z, m, cfg, p, g, cat, date, dec, ep).
Changer la palette de couleurs

Modifiez l'objet CAT_COLORS ou les variables CSS :root.
🤝 Contribution

Les contributions sont les bienvenues !

    Forkez le projet

    Créez une branche : git checkout -b feature/ma-fonctionnalite

    Committez : git commit -m "feat: ajout de ma fonctionnalité"

    Poussez : git push origin feature/ma-fonctionnalite

    Ouvrez une Pull Request

Merci de respecter la convention Conventional Commits.
🐛 Signaler un problème

Un bug ? Une suggestion ? Ouvrez une issue en précisant :

    Navigateur et version

    Étapes de reproduction

    Comportement attendu vs observé

    Capture d'écran si possible

📜 Licence

Ce projet est distribué sous licence MIT. Voir le fichier LICENSE pour plus d'informations.
text

MIT License — Copyright (c) 2024 gunout

👤 Auteur

gunout

    GitHub : @gunout

🙏 Remerciements

    Dmitri Mendeleïev pour la classification périodique originelle

    La communauté scientifique pour les données historiques et spectrales

    Toutes les personnes ayant contribué à l'amélioration de ce projet

<div align="center">

⭐ Si ce projet vous est utile, n'oubliez pas de lui attribuer une étoile ! ⭐

Fait pour la chimie, l'histoire des sciences et la pédagogie.
</div> ```
📋 Instructions

    Copiez l'intégralité du bloc markdown ci-dessus.

    Ouvrez votre dépôt : https://github.com/gunout/tableau-periodique-complet-version-numeration

    Cliquez sur README.md → ✏️ Edit

    Collez et Commit changes

Le README inclut :

    ✅ Badges professionnels (HTML5, CSS3, JS, MIT)

    ✅ Table des matières visuelle

    ✅ Sections structurées (Présentation, Fonctionnalités, Stack, Utilisation…)

    ✅ Tableau de correspondance alphabétique

    ✅ Instructions d'installation et de déploiement

    ✅ Guide de contribution

    ✅ Licence et remerciements
