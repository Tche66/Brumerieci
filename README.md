# 🚀 BRUMERIE - LANDING PAGE PRÉ-SEED

Landing page optimisée pour levée de fonds pré-seed et recrutement early adopters.

---

## ✨ CARACTÉRISTIQUES

### **Design**
- ✅ Minimaliste et professionnel
- ✅ Responsive mobile-first
- ✅ Animations smooth
- ✅ Carousel interactif screenshots Figma
- ✅ Vert émeraude (couleur Brumerie)

### **Sections**
1. **Hero** - Message clair : MVP en développement
2. **Early Traction** - 15 vendeurs + Prototype complet
3. **Carousel Figma** - 4 screenshots du prototype
4. **Le Problème** - 3 points data-driven
5. **La Solution** - 5 piliers de Brumerie
6. **Pourquoi Maintenant** - Timing + marché
7. **Roadmap** - Timeline Q1-Q4 2026
8. **Investisseurs** - Round structuré + formulaire
9. **Early Adopters** - Programme pilote + formulaire
10. **Fondateur** - Serge Alain + LinkedIn
11. **Avantage Compétitif** - 5 différenciateurs
12. **Footer** - Liens + légal

### **SEO**
- ✅ Meta tags complets
- ✅ Google Site Verification intégrée
- ✅ Open Graph (LinkedIn/Facebook)
- ✅ Sitemap.xml
- ✅ Robots.txt
- ✅ Balises sémantiques

### **Formulaires**
- ✅ 2 formulaires Formspree distincts
- ✅ Investisseurs → Pitch deck
- ✅ Early adopters → Programme pilote
- ✅ Validation automatique

---

## 📦 STRUCTURE

```
brumerie-preseed/
├── index.html          # Page complète (HTML + CSS + JS inline)
├── public/
│   ├── images/
│   │   ├── logo.png    # Logo Brumerie
│   │   ├── figma1.jpg  # Screenshot accueil
│   │   ├── figma2.jpg  # Screenshot produit
│   │   ├── figma3.jpg  # Screenshot profil
│   │   └── figma4.jpg  # Screenshot dashboard
│   ├── sitemap.xml
│   └── robots.txt
└── README.md
```

---

## 🚀 DÉPLOIEMENT

### **Option 1 : Netlify (Recommandé)**

#### **Via GitHub** :
1. Push ce dossier sur GitHub
2. Netlify.com → New site → Import from Git
3. Choisis le repo
4. Build settings : AUCUN (site statique)
5. Publish directory : `.` (racine)
6. Deploy

#### **Via Drag & Drop** :
1. Netlify.com → Sites → Add new site → Deploy manually
2. Glisse le dossier `brumerie-preseed/`
3. Attend 1 min → Site en ligne

### **Option 2 : Vercel**
```bash
npm i -g vercel
cd brumerie-preseed
vercel
```

### **Option 3 : GitHub Pages**
1. Push sur GitHub
2. Settings → Pages → Source: main branch
3. Site accessible sur `username.github.io/brumerie`

---

## 🌐 DOMAINE PERSONNALISÉ

### **Acheter brumerie.ci** (RECOMMANDÉ)
- **Prix** : ~15$/an
- **Où** : Hostinger, Namecheap, ou registraire .ci local

### **Configurer sur Netlify**
1. Netlify → Domain settings
2. Add custom domain → `brumerie.ci`
3. Ajouter les DNS chez ton registraire :
   ```
   Type: A
   Name: @
   Value: 75.2.60.5
   
   Type: CNAME
   Name: www
   Value: ton-site.netlify.app
   ```

---

## 📧 FORMULAIRES FORMSPREE

Les 2 formulaires utilisent **Formspree ID : `xkovnoqy`**

### **Emails reçus sur** :
`brumerieciv.email@gmail.com`

### **Différenciation** :
- Investisseurs : `type=investisseur`
- Early adopters : `type=early-adopter`

### **Si tu veux changer l'email** :
1. Va sur Formspree.io
2. Crée un nouveau formulaire
3. Remplace `xkovnoqy` dans les 2 forms par ton nouvel ID

---

## 🎨 PERSONNALISATION

### **Changer les couleurs**
Dans `index.html`, cherche `:root` et modifie :
```css
--emerald-500: #10b981;  /* Couleur principale */
--emerald-600: #059669;  /* Couleur hover */
```

### **Modifier les textes**
Tout est dans `index.html` - cherche les sections par titre :
- `<!-- Hero Section -->`
- `<!-- Investisseurs -->`
- etc.

### **Ajouter/retirer des images Figma**
1. Ajoute l'image dans `public/images/`
2. Dans le carousel, ajoute :
```html
<div class="carousel-slide">
  <img src="/images/figma5.jpg" alt="Description">
</div>
```
3. Ajoute un dot :
```html
<span class="dot" data-slide="4"></span>
```
4. Modifie `totalSlides = 5` dans le script

---

## 📊 ANALYTICS

### **Google Analytics** (Recommandé)
Ajoute avant `</head>` :
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXX');
</script>
```

### **Hotjar** (Optionnel)
Pour voir le comportement utilisateurs

---

## ✅ CHECKLIST POST-DÉPLOIEMENT

- [ ] Site déployé et accessible
- [ ] Tester les 2 formulaires
- [ ] Vérifier sur mobile
- [ ] Soumettre sitemap à Google Search Console
- [ ] Tester tous les liens (LinkedIn, Crunchbase)
- [ ] Partager sur LinkedIn
- [ ] Envoyer à FasterCapital
- [ ] Configurer domaine brumerie.ci

---

## 🎯 OBJECTIFS DE CETTE PAGE

1. **Lever 150k$** auprès d'investisseurs pré-seed
2. **Recruter 50+ early adopters** pour le MVP
3. **Crédibiliser Brumerie** auprès des partenaires
4. **Générer du trafic organique** via SEO

---

## 📈 MESURES DE SUCCÈS

### **Court terme (7 jours)**
- 10+ inscriptions early adopters
- 2+ contacts investisseurs
- Partages LinkedIn

### **Moyen terme (30 jours)**
- 50+ inscriptions early adopters
- 5+ meetings investisseurs
- Apparition Google "Brumerie CI"

---

## 🆘 SUPPORT

**Problème technique ?**
- Vérifie que toutes les images sont dans `public/images/`
- Teste en local avec `python3 -m http.server 8000`
- Ouvre `localhost:8000` dans ton navigateur

**Formulaires ne marchent pas ?**
- Vérifie l'ID Formspree : `xkovnoqy`
- Teste en envoyant un message
- Check ton email `brumerieciv.email@gmail.com`

---

## 🚀 PROCHAINES ÉTAPES

1. **Déploie immédiatement** sur Netlify
2. **Teste tout** (formulaires, liens, mobile)
3. **Achète brumerie.ci** (15$)
4. **Partage sur LinkedIn** avec le lien
5. **Envoie aux investisseurs** potentiels
6. **Soumets à Google** Search Console

---

**Fait avec 💚 pour le succès de Brumerie en Côte d'Ivoire**
