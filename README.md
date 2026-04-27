# NEON FRACTURE — Landing Page

> Site one-page immersif pour un jeu vidéo cyberpunk fictif, construit en HTML/CSS/JS vanilla avec Locomotive Scroll.

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Locomotive Scroll](https://img.shields.io/badge/Locomotive_Scroll-4.1.4-00f5ff?style=flat-square)

---

## Aperçu

**NEON FRACTURE** est un site promotionnel fictif pour un jeu de rôle cyberpunk se déroulant dans la mégalopole de *Nouvelle Vayne* en 2087. Le projet est une démonstration de techniques frontend avancées : effets visuels cyberpunk, animations au scroll, interactions personnalisées et typographie expressive.

Aucun framework. Aucune dépendance lourde. Un seul fichier HTML.

---

## Fonctionnalités

### Effets visuels
- **Curseur personnalisé** avec dot + anneau en lag, effets hover sur les éléments interactifs
- **Glitch animé** sur le titre hero (décalage chromatique par intervalles aléatoires)
- **Scanlines** animées en overlay sur toute la page
- **Grain / bruit** généré en SVG inline et animé en boucle
- **Grille de fond** fixe style terminal en CSS pur
- **Particles flottantes** générées dynamiquement en JS (40 particules colorées)
- **Flash hue-rotate** aléatoire sur le body pour simuler des artefacts visuels

### Scroll & animations
- **Locomotive Scroll 4.1.4** pour le défilement fluide (lerp 0.08)
- **IntersectionObserver** pour les révélations d'éléments au scroll (`data-reveal`)
- **Parallax** sur le contenu hero à l'entrée du scroll natif
- **Compteurs animés** (avec easing cubique) déclenchés à l'entrée de la section stats

### Composants UI
- **Navbar fixe** avec liens, logo et CTA — fond dégradé
- **Ticker** d'actualité en défilement CSS infini
- **Cards features** avec barre colorée au hover (clip-path hexagonal)
- **Runner cards expand** : flex 1 → flex 2.5 au hover, révélation des stats et citations
- **Districts grid** avec niveaux de menace en dots
- **Frame trailer** avec coins décoratifs, overlay SVG et bouton play animé
- **Boutons clip-path** en forme de parallélogramme

### Typographie
- `Bebas Neue` — titres display
- `Share Tech Mono` — labels, codes, données UI
- `Rajdhani` — corps de texte

---

## Structure du projet

```
neon_fracture.html        ← fichier unique, tout-en-un
```

Le projet est volontairement monolithique (HTML + CSS + JS dans un seul fichier) pour faciliter le déploiement et le partage.

---

## Sections de la page

| # | Section | Description |
|---|---------|-------------|
| 01 | **Hero** | Titre glitché, sous-titre, particules, scroll indicator |
| — | **Ticker** | Fil d'actualité défilant en continu |
| 02 | **Lore** | Histoire du jeu, grille hexagonale décorative |
| — | **Manifesto** | Citation typographique géante |
| 03 | **Gameplay** | 6 systèmes de jeu en grille |
| 04 | **Runners** | 4 classes jouables avec stats interactives |
| 05 | **Monde** | 4 districts de Nouvelle Vayne |
| 06 | **Trailer** | Frame cinématique décorative |
| — | **Stats** | Compteurs animés (4M runners, 200h contenu…) |
| — | **CTA** | Appel à l'action pré-commande |
| — | **Footer** | Logo, liens, copyright |

---

## Lancement

Aucune installation requise. Ouvre simplement le fichier dans un navigateur :

```bash
# Option 1 — ouvrir directement
open neon_fracture.html

# Option 2 — serveur local (recommandé pour Locomotive Scroll)
npx serve .
# ou
python -m http.server 8000
```

> ⚠️ Locomotive Scroll fonctionne mieux servi via HTTP. L'ouvrir en `file://` peut désactiver le scroll fluide.

---

## Dépendances externes

Chargées via CDN, aucune installation npm nécessaire.

| Lib | Version | Usage |
|-----|---------|-------|
| [Locomotive Scroll](https://locomotivemtl.github.io/locomotive-scroll/) | 4.1.4 | Smooth scroll |
| [Google Fonts](https://fonts.google.com) | — | Bebas Neue, Share Tech Mono, Rajdhani |

---

## Palette de couleurs

```css
--neon-cyan:   #00f5ff   /* couleur principale, hacks, UI */
--neon-pink:   #ff006e   /* danger, combat, accents chauds */
--neon-purple: #bf00ff   /* psynétique, Oracle */
--neon-yellow: #f5e642   /* tech, Vortex, warnings */
--neon-orange: #ff4d00   /* combat rapproché */
--dark:        #03020a   /* fond principal */
```

---

## Inspiration

- *Cyberpunk 2077* — esthétique visuelle et lore urbain
- *Cyberpunk: Edgerunners* — palette de couleurs saturées et énergie visuelle
- *Deus Ex* — interface UI diegétique
- *Nier: Automata* — typographie et philosophie narrative

---

## Licence

Projet fictif à but démonstratif. Contenu, personnages et univers entièrement inventés.  
Libre de réutilisation pour des projets personnels ou éducatifs.

---

<div align="center">
  <sub>// SIGNAL STUDIOS · WEBKRAFT · 2087 //</sub>
</div>
