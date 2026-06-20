---
name: INCA Suite
description: Suite opérationnelle d'import pour Groupe Incana — marché La Réunion
colors:
  navy-deep: "#0f1f5c"
  navy-mid: "#1e3a8a"
  blue-commerce: "#3b5bdb"
  blue-bright: "#4c6ef5"
  blue-soft: "#eef2ff"
  green-action: "#0ca678"
  green-soft: "#e6fcf5"
  orange-alert: "#e8590c"
  orange-soft: "#fff4e6"
  amber-caution: "#e67700"
  amber-soft: "#fff8e1"
  purple-badge: "#7048e8"
  purple-soft: "#f3f0ff"
  teal-info: "#0891b2"
  teal-soft: "#ecfeff"
  red-danger: "#e03131"
  red-soft: "#fff5f5"
  surface-bg: "#f0f4ff"
  surface-white: "#ffffff"
  border-default: "#e2e8f8"
  ink: "#0f172a"
  ink-mid: "#334155"
  ink-muted: "#64748b"
typography:
  display:
    fontFamily: "'Plus Jakarta Sans', sans-serif"
    fontSize: "clamp(28px, 5vw, 42px)"
    fontWeight: 800
    lineHeight: 1.1
    letterSpacing: "-1px"
  title:
    fontFamily: "'Plus Jakarta Sans', sans-serif"
    fontSize: "24px"
    fontWeight: 800
    lineHeight: 1.2
    letterSpacing: "-0.5px"
  body:
    fontFamily: "'Plus Jakarta Sans', sans-serif"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "'Plus Jakarta Sans', sans-serif"
    fontSize: "10px"
    fontWeight: 700
    letterSpacing: "2px"
  data-mono:
    fontFamily: "'JetBrains Mono', monospace"
    fontSize: "22px"
    fontWeight: 800
    lineHeight: 1.2
rounded:
  sm: "8px"
  md: "12px"
  lg: "16px"
  xl: "20px"
  pill: "20px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  section: "40px"
components:
  button-primary:
    backgroundColor: "{colors.blue-commerce}"
    textColor: "{colors.surface-white}"
    rounded: "{rounded.md}"
    padding: "14px 28px"
  button-primary-hover:
    backgroundColor: "{colors.blue-bright}"
    textColor: "{colors.surface-white}"
    rounded: "{rounded.md}"
    padding: "14px 28px"
  button-success:
    backgroundColor: "{colors.green-action}"
    textColor: "{colors.surface-white}"
    rounded: "{rounded.sm}"
    padding: "10px 20px"
  button-ghost:
    backgroundColor: "{colors.surface-white}"
    textColor: "{colors.green-action}"
    rounded: "{rounded.sm}"
    padding: "9px 16px"
  card-tool:
    backgroundColor: "{colors.surface-white}"
    rounded: "{rounded.lg}"
    padding: "24px"
  card-featured:
    backgroundColor: "{colors.surface-white}"
    rounded: "{rounded.xl}"
    padding: "32px 40px"
  chip-status:
    backgroundColor: "{colors.blue-soft}"
    textColor: "{colors.blue-commerce}"
    rounded: "{rounded.pill}"
    padding: "3px 9px"
---

# Design System: INCA Suite

## 1. Overview

**Creative North Star: "Le Tableau de Bord du Cargo"**

INCA Suite est un instrument de navigation professionnelle, pas une vitrine. Chaque pixel sert la décision : le coût de revient d'un article, le stock restant d'un lot, le score d'un produit fournisseur. L'interface emprunte son vocabulaire visuel au monde du fret maritime — bleus profonds, données monospaces, densité sans lourdeur — parce que c'est le contexte physique de l'outil : des conteneurs 40', DSG Transit, COMPROS La Possession.

Le registre est délibérément interne et professionnel. L'utilisateur sait ce qu'il cherche ; l'interface l'y amène sans cérémonies. Pas de tutoriels, pas de félicitations, pas d'empty states édifiants. Quand le stock est vide, on le dit. Quand un lot est périmé, on l'affiche en rouge. La densité est une fonctionnalité, pas un défaut.

Ce système rejette deux esthétiques : le **Dashboard BI clinquant** (graphiques partout, arrière-plans sombres saturés, performance visuelle au détriment de la lisibilité) et le **SaaS générique** (froid, interchangeable, conçu pour un marché mondial anonyme). INCA Suite opère à La Réunion, avec des taux de taxe locaux, des transitaires nommés (DSG Transit, Repiquet), un entrepôt précis — l'interface doit refléter cette spécificité, pas la masquer sous un vernis universel.

**Key Characteristics:**
- Fond bleu-lavande `#f0f4ff` — professionnel sans agressivité, jamais blanc pur ni gris neutre
- Header dégradé marine profond `#0f1f5c → #3b5bdb` comme ancrage visuel fort de chaque page
- Ombres teintées bleues — jamais neutres — qui ancrent les cartes dans la palette du site
- JetBrains Mono exclusivement pour les valeurs calculées, signal de fiabilité chiffrée
- Accents sémantiques stricts : vert action, orange vigilance, rouge urgence, violet nouveauté, teal info
- Densité assumée : tableaux et KPIs ne cherchent pas à paraître spacieux — ils sont là pour être lus vite

## 2. Colors: La Palette Cargo

Un système à deux couches : le **bleu commerce** comme fil directeur, et un ensemble d'**accents sémantiques** (vert, orange, rouge, violet, teal) utilisés exclusivement pour signaler un état ou une catégorie.

### Primary

- **Bleu Commerce Nocturne — dégradé header** (`#0f1f5c → #1e3a8a → #3b5bdb`, 135deg): Le seul gradient de surface du système. Exclusivement dans le header de chaque page. Évoque le fret maritime et la fiabilité institutionnelle. Ne jamais réutiliser ce gradient sur d'autres surfaces.
- **Bleu Commerce** (`#3b5bdb`): Couleur d'action primaire. Boutons principaux, CTA d'ouverture d'outil, focus states. La couleur que l'utilisateur clique.
- **Bleu Vif** (`#4c6ef5`): Variante hover du bleu commerce, légèrement plus lumineux pour signaler l'interactivité.
- **Bleu Doux** (`#eef2ff`): Surface informationnelle liée au bleu — badges, surlignages, fond de page. Jamais fond de carte principal.

### Secondary

- **Vert Action** (`#0ca678`): Toutes les actions liées au stock, aux entrées, aux validations, aux états positifs. La couleur "tout va bien" du système.
- **Vert Doux** (`#e6fcf5`): Fond des alertes vertes et badges positifs.

### Tertiary

- **Orange Alerte** (`#e8590c`): Lot DLC proche, réapprovisionnement nécessaire. Jamais décoratif.
- **Ambre Prudence** (`#e67700`): Niveau intermédiaire d'alerte — attention sans urgence critique.
- **Violet Badge** (`#7048e8`): Réservé aux indicateurs de nouveauté ou de feature principale. Usage parcimonieux.
- **Teal Info** (`#0891b2`): Informations secondaires, métriques complémentaires, widgets de données neutres.
- **Rouge Danger** (`#e03131`): Lots périmés, erreurs critiques, états bloquants. Toujours justifié.

### Neutral

- **Surface fond** (`#f0f4ff`): Fond de page. Bleu-lavande très léger, teinté vers la palette bleue — ni blanc pur ni gris neutre.
- **Surface blanche** (`#ffffff`): Fond des cartes et composants. Le contraste avec le fond de page crée la hiérarchie sans ombres excessives.
- **Bordure** (`#e2e8f8`): Séparateurs, bordures de cartes, dividers de tableaux. Même tonalité bleue que le fond.
- **Encre** (`#0f172a`): Texte principal. Quasi-noir avec légère teinte bleue — jamais noir pur `#000`.
- **Encre Médium** (`#334155`): Titres secondaires, valeurs de tableau importantes.
- **Encre Atténuée** (`#64748b`): Labels, descriptions, métadonnées. Contraste ≥ 4.5:1 sur fond blanc vérifié.

### Named Rules

**La Règle du Sémantique Strict.** Les couleurs d'accent (vert, orange, rouge, violet, teal) ne sont jamais décoratives. Chaque occurrence signale un état métier précis. Si l'hésitation est entre deux couleurs d'accent, c'est que la situation n'est pas assez définie — on clarifie d'abord, on colore ensuite.

**La Règle de l'Ombre Bleue.** Les ombres portées ne sont pas neutres dans ce système. Elles sont teintées bleu (`rgba(59,91,219,.07-.15)`) pour rester en tonalité avec la palette. Des ombres grises-noires sur fond `#f0f4ff` créent une discordance tonale.

## 3. Typography

**Display Font:** Plus Jakarta Sans (Google Fonts — 400, 500, 600, 700, 800)
**Data Font:** JetBrains Mono (Google Fonts — 400, 500, 600)

**Character:** Plus Jakarta Sans au poids 800 est le moteur de l'identité visuelle — géométrique, légèrement humaniste, lisible à haute densité sans paraître froid. JetBrains Mono, utilisé exclusivement pour les chiffres clés, signale immédiatement que ces valeurs sont issues d'un calcul précis, pas d'une estimation tapée à la main.

### Hierarchy

- **Display** (800, clamp(28px, 5vw, 42px), lh 1.1, ls -1px): Titre de page dans le header. Une seule occurrence par page.
- **Title** (800, 24px, lh 1.2, ls -0.5px): Titre des featured cards et sections majeures.
- **Subtitle** (800, 20px, lh 1.2, ls -0.3px): Titres de widgets et blocs secondaires.
- **Body** (400–500, 14–15px, lh 1.6): Descriptions de cartes, contenu de tableau, sous-titres de header. Max 520px de largeur sur les blocs de texte long.
- **Label** (700, 10px, ls 2px, uppercase): Section labels, en-têtes de colonnes de tableau, sous-titres de KPI. Toujours accompagné d'un élément graphique (ligne horizontale ou icône).
- **Data Mono** (JetBrains Mono 800, 20–22px): Valeurs KPI, métriques dans le header, totaux stock. Exclusivement pour les nombres calculés.
- **Micro** (600–700, 9–12px, ls 0.5px): Tags, status badges, footnotes de tableaux.

### Named Rules

**La Règle du Mono Calculé.** JetBrains Mono n'apparaît que sur des valeurs sorties d'un calcul ou d'une base de données (CRR, totaux, volumes, prix). Un chiffre tapé à la main reste en Plus Jakarta Sans.

## 4. Elevation

Le système utilise des **ombres structurelles légères teintées bleues**. La hiérarchie est binaire : cartes au repos et cartes en survol. Pas d'élévation matérielle à niveaux multiples. Toutes les surfaces de cartes ont une ombre — il n'y a pas de surface "plate sans ombre" dans ce système.

### Shadow Vocabulary

- **Ombre repos** (`0 1px 4px rgba(59,91,219,.08), 0 8px 24px rgba(59,91,219,.07)`): Toutes les cartes, widgets et panneaux à l'état par défaut. Double couche : micro-ombre de contact + ombre portée diffuse bleue.
- **Ombre survol** (`0 4px 20px rgba(59,91,219,.15), 0 12px 40px rgba(59,91,219,.1)`): État hover des cartes cliquables. Le rayon s'élargit et la teinte bleue s'intensifie.

### Named Rules

**La Règle de l'Élévation Responsive.** Les ombres sont présentes au repos et s'amplifient à l'état actif — jamais l'inverse. Une carte cliquable doit toujours avoir une ombre au repos pour signaler son interactivité avant même le survol.

## 5. Components

### Buttons

Deux familles : **action primaire** (bleu, ouverture d'outil) et **action contextuelle** (vert pour le stock, fantôme pour les actions secondaires).

- **Shape:** Légèrement arrondies (12px pour les boutons principaux, 10px pour les boutons secondaires)
- **Primary (bleu):** Fond gradient `#3b5bdb → #4c6ef5`, texte blanc, padding 14px 28px, ombre bleue `rgba(59,91,219,.35)`. Transition `scale(1.03)` au hover. Usage : CTA d'ouverture d'outil, navigation principale.
- **Success (vert):** Fond gradient `#0ca678 → #0d9e72`, texte blanc, padding 10px 20px. Ombre verte `rgba(12,166,120,.3)`. Usage : actions stock (ouvrir, saisir, gérer).
- **Ghost (contour vert):** Fond blanc, bordure 1.5px `#0ca678`, texte `#0ca678`, padding 9px 16px. Fond `green-soft` au hover. Usage : actions secondaires (export CSV, actions alternatives).

### Chips & Badges

- **Status badge (cellule de tableau):** Fond sémantique doux, texte couleur assortie, padding 2px 7px, radius 8px, font 10px 700.
- **Module badge (header de widget):** Fond gradient doux entre deux teintes douces (ex: `blue-soft → purple-soft`), bordure transparente 20% de la couleur principale, radius 20px (pill), font 10px 700 ls 0.5px.
- **Section badge (featured card):** Même style que module badge, légèrement plus visible — utilisé pour les indicateurs de nouveauté.
- **Status tag (outil grid):** Fond coloré doux, texte couleur forte, radius 20px, font 9px 700. Stable = `blue-soft/blue`, New = gradient vert, Beta = `amber-soft/amber`.

### Cards

Cœur du système. Deux gabarits principaux.

- **Tool Card (grille):** Fond blanc, radius 16px, padding 24px, ombre repos. Flexbox colonne avec gap 16px. Icône 48×48px dans un carré arrondi 12px coloré (fond doux de la couleur d'accent). Flèche `→` en bas à droite (32×32px, radius 8px, fond `surface-bg`) qui devient bleu au hover de la carte. Bordure haut du footer: `border-default` 1px.
- **Featured Card:** Fond blanc, radius 20px, padding 32px 40px. Barre accent 4px en haut avec gradient `#3b5bdb → #4c6ef5 → #7048e8`. Grid 2 colonnes (contenu + CTA). La barre du haut est l'élément distinctif — réservée aux featured cards et widgets de niveau "featured". Jamais sur les tool cards standards.
- **KPI Card (mini):** Fond `surface-bg`, radius 12px, padding 14px 16px. Valeur en JetBrains Mono 20px 800, label en 10px uppercase `ink-muted`. La couleur de la valeur change sémantiquement (green/orange/red/blue) selon l'état du KPI.
- **Info Bar:** Fond blanc, radius 14px, padding 20px 24px. Flex horizontal aligné. Icône + bloc texte (titre 13px 700 + sous-titre 11px `ink-muted`) + bouton action en bout de ligne.

### Data Tables

- **Header:** Fond `surface-bg`, texte `ink-muted` 10px uppercase ls 0.5px, position sticky top. Bordure basse `border-default`. Padding 8px 16px par cellule.
- **Lignes:** Bordure basse `border-default`, hover fond `surface-bg` (transition 0.1s). Texte 12px. Valeurs importantes en `<strong>`, détails complémentaires en `ink-muted` 10px sur une deuxième ligne dans la même cellule.
- **Badges dans cellules:** Mêmes status badges sémantiques que partout dans le système (green=OK, orange=réappro, red=périmé, gray=épuisé).
- **Max-height:** Les tableaux embarqués dans des widgets ont un `max-height: 240px` avec scroll interne.

### Section Labels

Séparateur de groupe : texte 10px 700 uppercase `ink-muted` ls 2px, suivi d'une ligne `border-default` flex-1. Existe pour séparer des groupes logiques distincts — pas un décor répétitif entre chaque élément.

## 6. Do's and Don'ts

### Do:

- **Do** utiliser JetBrains Mono exclusivement pour les valeurs calculées (CRR, totaux, volumes, prix calculés). Jamais pour du texte courant.
- **Do** teinter toutes les ombres en bleu (`rgba(59,91,219,...)`) — les ombres grises sur fond `#f0f4ff` créent une discordance tonale.
- **Do** réserver chaque couleur d'accent à son état sémantique : vert = action/succès, orange = vigilance, rouge = urgence, violet = nouveauté, teal = info. Zéro usage décoratif.
- **Do** utiliser `transform: translateY(-2px)` + amplification d'ombre pour toutes les cartes cliquables au hover.
- **Do** afficher les chiffres avec leur unité : toujours `€`, `u`, `j`, `%`, `k€` — jamais un nombre seul sur des valeurs métier.
- **Do** laisser les blocs de texte corps à max 520px et line-height 1.6 — la densité de données ne justifie pas de sacrifier la lisibilité.

### Don't:

- **Don't** reproduire l'esthétique Dashboard BI clinquant : pas de fond sombre saturé de graphiques, pas de "big number with gradient glow" (le hero-metric template), pas de neons, pas de glassmorphisme décoratif.
- **Don't** reproduire l'esthétique SaaS générique (Notion/Linear/Vercel) : pas de surfaces ultra-minimalistes sans caractère, pas de typographie neutre sans ancrage. L'outil est local et spécifique.
- **Don't** utiliser les couleurs d'accent (vert, orange, violet, teal, rouge) de façon décorative. Chaque occurrence doit être justifiable par un état métier.
- **Don't** ajouter des ombres neutres (grises ou noires). Toutes les ombres sont teintées `rgba(59,91,219,...)`.
- **Don't** utiliser `border-left` ou `border-right` > 1px comme accent coloré. La barre de couleur est toujours en haut (4px, `top: 0; left: 0; right: 0`), jamais latérale.
- **Don't** multiplier les section labels à uppercase sur chaque élément — ils séparent des groupes logiques, pas chaque composant individuel.
- **Don't** afficher un gradient de texte (`background-clip: text`). Tout texte est en couleur pleine.
- **Don't** utiliser des grilles de cards identiques sans variation de gabarit. Alterner featured card + grille tool cards, ou widget spécialisé + grille, donne la hiérarchie visuelle nécessaire.
