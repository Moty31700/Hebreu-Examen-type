# מבחן עברית A1 — Examen Hébreu Interactif

Application web progressive (PWA) pour l'examen de fin de semestre hébreu niveau A1.  
**Installable sur iPad, iPhone et Android** sans passer par l'App Store.

---

## 📱 Installation sur iPad / iPhone

1. Ouvrir l'URL de l'app dans **Safari**
2. Appuyer sur l'icône **Partager** (carré avec flèche ↑)
3. Choisir **"Sur l'écran d'accueil"**
4. L'app s'installe comme une vraie application, utilisable **hors-ligne**

## 📱 Installation sur Android

1. Ouvrir l'URL dans **Chrome**
2. Chrome affiche automatiquement une bannière "Ajouter à l'écran d'accueil"
3. Ou : menu ⋮ → "Ajouter à l'écran d'accueil"

---

## 🚀 Déploiement sur GitHub Pages (gratuit)

### Option 1 — Interface GitHub (sans ligne de commande)

1. Créer un compte sur [github.com](https://github.com) si besoin
2. Cliquer **"New repository"** → nommer le dépôt `mivhan-a1` → **"Create repository"**
3. Cliquer **"uploading an existing file"**
4. Glisser-déposer **tous les fichiers** de ce dossier :
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - dossier `icons/` (avec les 3 fichiers PNG/SVG)
5. Cliquer **"Commit changes"**
6. Aller dans **Settings → Pages**
7. Source : **"Deploy from a branch"** → branche `main` → dossier `/root`
8. Cliquer **Save**

✅ L'app sera disponible sur :  
`https://VOTRE_NOM.github.io/mivhan-a1/`

### Option 2 — Terminal (si Git installé)

```bash
cd mivhan-a1-pwa
git init
git add .
git commit -m "Initial commit — Mivhan A1 PWA"
git branch -M main
git remote add origin https://github.com/VOTRE_NOM/mivhan-a1.git
git push -u origin main
```
Puis activer GitHub Pages dans Settings → Pages.

---

## 📚 Contenu de l'examen

| Partie | Contenu | Points |
|--------|---------|--------|
| 1 | Pronoms personnels (pronoms manquants) | 3 pts |
| 2 | Verbes — tableau de conjugaison | 3 pts |
| 3 | Présentatifs זֶה / זֹאת / אֵלֶּה | 2 pts |
| 4 | Chiffres (hébreu → chiffre) | 2 pts |
| 5 | Singulier ↔ Pluriel | 2 pts |
| 6 | Compréhension écrite (Yossi à Madrid) | 4 pts |
| 7 | Expression écrite libre | 4 pts |
| **Total** | | **20 pts** |

## ⚙️ Fonctionnement de la correction

- **1ʳᵉ passe** : les réponses fausses sont surlignées en **jaune** → correction possible
- **2ᵉ passe** : les cases encore fausses passent en **rouge**, la bonne réponse s'affiche
- **Score** : plein si juste au 1er essai, moitié au 2ᵉ, zéro sinon
- **Offline** : fonctionne sans connexion après le premier chargement

---

## 🛠 Technologies

- HTML5 / CSS3 / JavaScript vanilla
- PWA (Service Worker + Web App Manifest)
- Police : Noto Serif Hebrew + Crimson Pro (Google Fonts)
- Aucune dépendance externe, aucun framework

## 📝 Licence

Usage pédagogique libre. Créé avec Claude (Anthropic).
