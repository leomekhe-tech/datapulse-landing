# DataPulse Landing Page

## 🎨 Design System

### Couleurs
- **Primary**: #0EA5E9 (Sky Blue)
- **Secondary**: #6366F1 (Indigo)
- **Accent**: #22D3EE (Cyan)
- **Dark**: #0F172A (Slate 900)
- **Light**: #F8FAFC (Slate 50)
- **Success**: #10B981

### Typographie
- Font: Inter (Google Fonts)
- Weights: 400, 500, 600, 700, 800

---

## 📝 Copy Sections

### Hero
- **Headline**: "Observability for dbt + Airflow"
- **Subtitle**: "Stop guessing why your data pipelines break. Get real-time alerts, lineage tracking, and root cause analysis in one dashboard."
- **Badge**: "Early Access — Join 50+ data teams"

### Problem
- **Title**: "Data pipelines fail silently"
- **Subtitle**: "Your stakeholders notice broken dashboards before you do. Sound familiar?"

1. **Silent Failures**: "dbt tests pass but dashboards show stale data. Airflow tasks fail at 2 AM and nobody knows until the CEO asks."
2. **No Root Cause**: "When pipelines break, you spend hours digging through logs across dbt, Airflow, and your warehouse. Time you don't have."
3. **Reactive Firefighting**: "You're always playing catch-up. By the time you fix one issue, three more have popped up downstream."

### Solution
- **Title**: "Complete pipeline visibility"
- **Subtitle**: "DataPulse monitors your entire data stack and tells you exactly what's wrong, before your stakeholders do."

Features:
1. **Unified Dashboard**: "See dbt models, Airflow DAGs, and data quality metrics in one place. No more tab switching."
2. **Real-time Alerts**: "Get notified in Slack when tests fail, runs are late, or anomalies are detected. Customizable and actionable."
3. **Column-level Lineage**: "Trace any data issue back to its source. Understand impact before making changes."
4. **Smart Debugging**: "AI-powered root cause analysis that points you to the exact model, task, or schema change causing issues."
5. **Cost Monitoring**: "Track warehouse spend by model and user. Identify expensive queries before they blow your budget."
6. **Security & Governance**: "Monitor access patterns, detect PII exposure risks, and maintain audit trails automatically."

### Pricing
- **Title**: "Simple, transparent pricing"
- **Subtitle**: "Start free, scale as you grow. No hidden fees, no surprises."

**Starter ($0)**
- 1 connected warehouse
- Up to 100 models
- 7-day data retention
- Email alerts
- Community support

**Team ($99/mo)**
- Unlimited warehouses
- Unlimited models
- 90-day data retention
- Slack + PagerDuty alerts
- Column-level lineage
- Priority support

**Enterprise (Custom)**
- Everything in Team
- Unlimited retention
- SSO & advanced security
- Custom integrations
- Dedicated success manager
- SLA guarantee

---

## 🔧 Technical Stack

- **Hosting**: GitHub Pages (100% free)
- **Form**: Tally.so (free tier, unlimited responses)
- **Font**: Google Fonts (Inter)
- **Icons**: Emoji + CSS gradients (no external dependencies)

### Performance
- Single HTML file (~15KB)
- No JavaScript dependencies except Tally embed
- Lazy loading on iframe
- CSS inlined for fastest render
- Target load time: < 1s on 3G

---

## 📁 File Structure

```
datapulse-landing/
├── index.html          # Main landing page
├── logo-400x400.png    # Logo (copied from output/)
├── README.md           # This file
└── .nojekyll           # Disable Jekyll processing
```

---

## 🚀 Deployment

### Option 1: GitHub Pages (Recommended)
1. Create repo `datapulse-landing`
2. Push files to `main` branch
3. Enable GitHub Pages in Settings → Pages
4. Choose "Deploy from branch" → `main` → `/ (root)`
5. Site live at `https://yourusername.github.io/datapulse-landing/`

### Option 2: Netlify Drop
1. Zip the folder
2. Go to netlify.com/drop
3. Drag & drop zip
4. Instant deploy with custom domain support

### Option 3: Vercel
1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in folder
3. Follow prompts

---

## 📧 Email Capture Setup

**Tally.so Form** (déjà intégré)
- Form ID: `w7X9y5`
- Dashboard: https://tally.so/forms/w7X9y5
- Notifications: email alerts for new submissions
- Export: CSV/PDF/Excel

Pour modifier le form:
1. Se connecter à Tally.so
2. Ouvrir le form "DataPulse Waitlist"
3. Modifier champs/questions
4. Les changements apparaissent automatiquement sur la landing page

---

## 🎯 SEO Checklist

✅ Title tag: "DataPulse — Observability for dbt + Airflow pipelines"
✅ Meta description (155 chars)
✅ Open Graph tags
✅ Favicon (logo-100x100.png)
✅ Semantic HTML structure
✅ Mobile-responsive
✅ Fast load time

---

## 📱 Responsive Breakpoints

- **Desktop**: 1200px+ (full layout)
- **Tablet**: 768px - 1199px (2 columns)
- **Mobile**: < 768px (single column, adjusted typography)

---

## 🔮 Future Enhancements

- [ ] A/B testing with Google Optimize
- [ ] Analytics with Plausible (privacy-friendly)
- [ ] Live chat widget (Crisp/Intercom free tier)
- [ ] Demo video embed
- [ ] Testimonials section
- [ ] Integration logos (Snowflake, BigQuery, etc.)

---

## 📝 Changelog

**v1.0** - 2025-03-06
- Initial landing page
- Tally.so form integration
- Responsive design
- GitHub Pages ready
