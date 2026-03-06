# DataPulse Landing Page — Documentation

## 🚀 URL Live

**Production:** https://datapulse-landing.vercel.app

---

## 📋 Résumé

Landing page complète pour DataPulse — outil d'observability pour pipelines dbt + Airflow.

### Stack Technique
| Composant | Technologie |
|-----------|-------------|
| **Hosting** | Vercel (CDN global, HTTPS gratuit) |
| **Form** | Formspree (50 soumissions/mois gratuites) |
| **Font** | Google Fonts (Inter) |
| **Icons** | Emoji natifs (aucune dépendance externe) |

### Performance
- **Load time:** < 1s (fichier HTML unique, ~23KB)
- **Lighthouse:** 95+ expected (pas de JS lourd, CSS inlined)
- **Mobile-first:** Responsive breakpoints à 768px

---

## 🎨 Design System

### Palette Couleurs
```css
--primary: #0EA5E9      /* Sky Blue - actions principales */
--secondary: #6366F1    /* Indigo - accents */
--accent: #22D3EE       /* Cyan - highlights */
--dark: #0F172A         /* Slate 900 - fond hero/pricing */
--light: #F8FAFC        /* Slate 50 - fond sections */
--success: #10B981      /* Vert - badges/CTA */
```

### Structure de la Page
1. **Hero** — Logo, headline, sous-titre, formulaire email
2. **Problem** — 3 cartes de pain points
3. **Solution** — 6 features avec icons
4. **Pricing** — 3 plans (Starter/Team/Enterprise)
5. **Footer CTA** — Call-to-action final

---

## 📧 Email Capture

### Formspree Configuration
- **Endpoint:** `https://formspree.io/f/xblgkwjv`
- **Champs:** email (required), company (optional)
- **Notifications:** Configurées dans le dashboard Formspree
- **Limites:** 50 soumissions/mois (plan gratuit)

### Accéder aux soumissions
1. Aller sur https://formspree.io/forms/xblgkwjv
2. Se connecter avec le compte GitHub (leomekhe-tech)
3. Voir les soumissions en temps réel
4. Exporter en CSV si besoin

### Upgrade si nécessaire
- **Gold ($8/mois):** 1,000 soumissions, pas de branding Formspree
- **Dashboard:** https://formspree.io/account

---

## 📝 Modification du Contenu

### Option 1: Local + Git
```bash
cd /root/.openclaw/workspace/output/datapulse-landing
# Modifier index.html
nano index.html
# Commit et deploy
git add . && git commit -m "Update content"
npx vercel --prod
```

### Option 2: GitHub + Vercel Dashboard
1. Modifier sur GitHub: https://github.com/leomekhe-tech/datapulse-landing
2. Vercel auto-deploy sur chaque push

### Sections modifiables

#### Hero (ligne ~85)
```html
<h1>Observability for <span>dbt + Airflow</span></h1>
<p class="hero-subtitle">Votre texte ici...</p>
```

#### Problem Cards (ligne ~140)
Modifier les titres et descriptions dans les `.problem-card`

#### Pricing (ligne ~280)
Modifier les prix et features dans les `.pricing-card`

---

## 🖼️ Assets

### Logo
- **Fichier:** `logo-400x400.png`
- **Format:** PNG avec fond transparent
- **Usage:** Hero section, favicon

### Remplacer le logo
1. Générer nouveau logo (400x400px minimum)
2. Remplacer `logo-400x400.png`
3. Commit + push → auto-deploy

---

## 📱 Responsive

### Breakpoints
- **Desktop:** 1200px+ (layout complet)
- **Tablet:** 768px - 1199px (2 colonnes)
- **Mobile:** < 768px (1 colonne, typo réduite)

### Test responsive
```bash
# Ouvrir les DevTools (F12)
# Toggle device toolbar (Ctrl+Shift+M)
# Sélectionner iPhone SE / iPhone 12 Pro / Pixel 5
```

---

## 🔍 SEO

### Meta Tags configurés
- **Title:** "DataPulse — Observability for dbt + Airflow pipelines"
- **Description:** 155 caractères, mots-clés ciblés
- **Open Graph:** Pour partage LinkedIn/Twitter
- **Favicon:** `logo-100x100.png`

### Améliorations futures
- [ ] Ajouter Schema.org JSON-LD
- [ ] Google Analytics 4
- [ ] Plausible Analytics (privacy-friendly)
- [ ] Sitemap.xml

---

## 🌐 Custom Domain (Optionnel)

Pour utiliser `datapulse.io` ou `getdatapulse.com`:

### Via Vercel Dashboard
1. Aller sur https://vercel.com/dashboard
2. Sélectionner projet `datapulse-landing`
3. Settings → Domains
4. Add Domain → Entrer le domaine
5. Configurer DNS chez le registrar (Cloudflare/Namecheap/etc.)

### DNS Records nécessaires
```
Type: A | Name: @ | Value: 76.76.21.21
Type: CNAME | Name: www | Value: cname.vercel-dns.com
```

---

## 🔄 Backup & Recovery

### Repository GitHub
- **URL:** https://github.com/leomekhe-tech/datapulse-landing
- **Backup automatique:** Chaque commit est versionné

### Restauration
```bash
git clone https://github.com/leomekhe-tech/datapulse-landing.git
cd datapulse-landing
npx vercel --prod
```

---

## 📊 Analytics & Suivi

### Formspree (activé)
- Nombre de soumissions
- Taux de conversion
- Export CSV

### À ajouter si besoin
```html
<!-- Plausible (privacy-friendly) -->
<script defer data-domain="datapulse-landing.vercel.app" src="https://plausible.io/js/script.js"></script>

<!-- Google Analytics 4 -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXX"></script>
```

---

## 🆘 Troubleshooting

### Le site ne s'affiche pas
1. Vérifier URL: https://datapulse-landing.vercel.app
2. Vérifier statut Vercel: https://vercel.com/dashboard
3. Vérifier build logs dans Vercel dashboard

### Le formulaire ne fonctionne pas
1. Vérifier endpoint Formspree dans le HTML
2. Tester avec un email valide
3. Vérifier spam folder dans Formspree dashboard

### Le logo ne s'affiche pas
1. Vérifier que `logo-400x400.png` existe dans le repo
2. Vérifier le chemin dans le HTML: `./logo-400x400.png`
3. Faire un hard refresh (Ctrl+Shift+R)

---

## 📞 Contact & Support

- **Vercel Dashboard:** https://vercel.com/dashboard
- **Formspree Dashboard:** https://formspree.io/account
- **GitHub Repo:** https://github.com/leomekhe-tech/datapulse-landing

---

**Dernière mise à jour:** 2025-03-06
**Version:** 1.0
