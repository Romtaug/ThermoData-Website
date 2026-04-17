# ThermoData — Checklist SEO & déploiement

## ✅ Ce qui est fait dans `index.html`

### Meta tags essentielles
- [x] `<title>` optimisée (65 caractères, mot-clé principal + marque)
- [x] `<meta description>` (155 caractères, accroche + CTA implicite)
- [x] `<meta keywords>` (20 mots-clés ciblés secteur rénovation/RGE)
- [x] `<meta author>`, `<meta robots>`, `<meta language>`
- [x] `<html lang="fr">` + `hreflang` (fr-FR + x-default)
- [x] `<link rel="canonical">`
- [x] Geo tags (Lyon, FR-ARA, coordonnées GPS)

### Open Graph (Facebook, LinkedIn, WhatsApp…)
- [x] `og:type`, `og:site_name`, `og:title`, `og:description`
- [x] `og:url`, `og:locale`
- [x] `og:image` (1200×630, type, alt) — **À créer : `assets/og-image.png`**

### Twitter Cards
- [x] `twitter:card` (summary_large_image)
- [x] `twitter:site`, `twitter:creator` — **À ajuster : handle Twitter réel**
- [x] `twitter:title`, `twitter:description`, `twitter:image`

### Schema.org JSON-LD (rich snippets Google)
- [x] **Organization** (nom, logo, SIRET, adresse, contact)
- [x] **LocalBusiness** (Lyon + coordonnées GPS)
- [x] **WebSite** (avec publisher lié)
- [x] **Product** (AggregateOffer, 3 offres, prix réels)
- [x] **Service** (prospection B2B)
- [x] **BreadcrumbList** (6 niveaux)
- [x] **FAQPage** (7 questions → éligible rich snippet FAQ Google)
- [x] **HowTo** (9 étapes du pipeline → éligible rich snippet)
- [x] **VideoObject** (démo Loom)

### HTML5 sémantique
- [x] `<header>`, `<main>`, `<footer>`, `<nav>`, `<section>`, `<article>`, `<aside>`
- [x] Hiérarchie `<h1>` → `<h2>` → `<h3>` respectée (1 seul H1)
- [x] `<ol>` pour timeline + étapes (ordre sémantique)
- [x] Microdata inline sur prix (itemscope/itemtype/itemprop)
- [x] Microdata Organization sur footer

### Accessibilité (= bonus SEO)
- [x] `aria-label` sur tous les boutons/CTA
- [x] `aria-expanded` dynamique sur burger menu + FAQ
- [x] `aria-labelledby` reliant sections et titres
- [x] `aria-hidden="true"` sur décoratifs (SVG, icônes)
- [x] Skip link "Aller au contenu principal"
- [x] `role="banner"`, `role="main"`, `role="contentinfo"`, `role="navigation"`
- [x] Alt text descriptif sur toutes les images
- [x] `width`/`height` explicites sur images (anti-CLS)
- [x] `fetchpriority="high"` sur le logo hero

### Performance
- [x] `preconnect` Google Fonts + Loom
- [x] `dns-prefetch` Stripe + Google Docs + Streamlit
- [x] `preload` logo critique
- [x] `loading="lazy"` sur iframe Loom
- [x] `rel="noopener noreferrer"` sur tous les liens externes

### Fichiers SEO complémentaires créés
- [x] `robots.txt` (avec directives bots IA + sitemap)
- [x] `sitemap.xml` (avec hreflang + images)
- [x] `manifest.json` (PWA avec shortcuts)

---

## ⚠️ À FAIRE avant déploiement

### 1. Image Open Graph (CRITIQUE)
Créer `/assets/og-image.png` en **1200×630 pixels** avec :
- Le logo ThermoData
- Le slogan principal
- Un visuel de carte ou d'Excel
- Format PNG ou JPG, < 300 Ko idéalement

Outils recommandés : Figma, Canva, [og-image.vercel.app](https://og-image.vercel.app/)

### 2. Handles réseaux sociaux
Dans `index.html`, remplacer `@thermodata_fr` par ton handle Twitter/X réel (ou supprimer ces 2 lignes si pas de compte).

### 3. Google Search Console
- [ ] Valider la propriété `https://thermodata.fr/`
- [ ] Soumettre `sitemap.xml`
- [ ] Vérifier l'indexation

### 4. Google Business Profile (CRITIQUE pour le local)
- [ ] Créer une fiche GBP pour ThermoData à Lyon
- [ ] Catégorie : "Service de marketing" ou "Consultant en marketing"
- [ ] Ajouter photos, horaires, description
- [ ] Demander des avis clients

### 5. Tests et validation
- [ ] **Rich Results Test** : https://search.google.com/test/rich-results
  → Vérifier FAQPage, Product, HowTo, Organization
- [ ] **PageSpeed Insights** : https://pagespeed.web.dev/
  → Viser 90+ sur mobile et desktop
- [ ] **Schema Markup Validator** : https://validator.schema.org/
- [ ] **Mobile-Friendly Test** : https://search.google.com/test/mobile-friendly

### 6. Analytics
Ajouter juste avant `</head>` :
- Google Analytics 4 (ou Plausible/Simple Analytics pour RGPD-friendly)
- Google Tag Manager si multi-outils

---

## 📊 Mots-clés ciblés (par ordre d'importance)

**Tête longue (fort volume, concurrentiel)**
1. prospection artisan RGE
2. données DPE
3. passoires thermiques
4. rénovation énergétique leads

**Longue traîne (volume moyen, fort ROI)**
5. plan prospection chauffagiste
6. adresses passoires thermiques
7. fichier DPE ADEME prospection
8. prospection porte à porte rénovation
9. leads qualifiés artisan RGE
10. liste logement classe F G

**Local (faible concurrence, fort taux de conversion)**
11. prospection artisan RGE Lyon
12. données DPE [département]
13. prospection rénovation énergétique Rhône-Alpes

---

## 🎯 Stratégie de contenu SEO (prochaines étapes)

Pour exploser sur Google, créer un blog avec ces articles :

1. **"Comment trouver les passoires thermiques dans votre département"** (guide pratique)
2. **"DPE : comprendre les classes F et G et les obligations légales 2025-2034"** (pilier)
3. **"Prospection porte-à-porte : techniques pour artisans RGE en 2026"**
4. **"MaPrimeRénov' 2026 : guide complet pour artisans et propriétaires"**
5. **"Comment utiliser l'open data ADEME pour développer son activité"**
6. **Études de cas** (si tes clients acceptent) : "Comment [Entreprise X] a signé 12 chantiers en 2 mois avec ThermoData"

Chacun de ces articles doit :
- Faire 1500+ mots
- Inclure une infographie ou un visuel original
- Avoir un meta-titre < 60 caractères
- Être interlinké vers la page d'accueil et vers les autres articles
- Avoir son propre Schema.org Article

---

## 🔗 Netlinking prioritaire

Cibles pour obtenir des backlinks (par ordre de priorité) :
1. **France Rénov'** (référence officielle)
2. **Capeb** (confédération artisans bâtiment)
3. **FFB** (Fédération Française du Bâtiment)
4. **Qualibat / Qualit'EnR** (organismes RGE)
5. Blogs d'artisans et éditeurs logiciels BTP
6. Annuaires spécialisés rénovation (Habitatpresto, Rénov' Primes…)
7. Forums et groupes Facebook d'artisans RGE

---

## 📱 Signaux sociaux

- [ ] LinkedIn : page entreprise ThermoData
- [ ] Instagram : portfolio visuel (cartes, Excel)
- [ ] TikTok / YouTube Shorts : démos 30s

Publier 2-3 fois / semaine du contenu éducatif autour du DPE et de la rénovation.
