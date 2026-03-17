# 🚐 Fleet Management DHL

Application web progressive (PWA) pour la gestion de l'autonomie de la flotte électrique DHL.

## ✅ Fonctionnalités

- 🔐 Connexion par administrateur (Mike, Steve, Rachel, Erwin)
- 📊 Tableau de bord avec graphiques d'évolution
- ✍️ Saisie journalière (autonomie + chauffeur + véhicule non utilisé)
- 🚐 Gestion de la flotte (7 camionnettes pré-chargées)
- 👥 Liste de 27 coursiers (= chauffeurs)
- 📄 Rapports PDF avec chauffeur J-2 responsable
- 📲 **Installable sur smartphone et PC**

---

## 🚀 Déploiement sur GitHub Pages (gratuit)

### Étape 1 — Créer le dépôt GitHub

1. Aller sur [github.com](https://github.com) → Se connecter ou créer un compte
2. Cliquer sur **"New repository"** (bouton vert +)
3. Nom du dépôt : `dhl-fleet-management` (ou ce que vous voulez)
4. Cocher **"Public"** (obligatoire pour GitHub Pages gratuit)
5. Cliquer **"Create repository"**

### Étape 2 — Uploader les fichiers

**Option A — Interface web (le plus simple) :**
1. Dans votre dépôt, cliquer **"uploading an existing file"**
2. Glisser-déposer **tous les fichiers** du dossier dézippé :
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - Le dossier `icons/` (avec icon-192.png et icon-512.png)
   - Le dossier `.github/` (avec workflows/deploy.yml)
3. Cliquer **"Commit changes"**

**Option B — Git en ligne de commande :**
```bash
cd dhl_fleet_management
git init
git add .
git commit -m "Initial deploy"
git branch -M main
git remote add origin https://github.com/VOTRE_USERNAME/dhl-fleet-management.git
git push -u origin main
```

### Étape 3 — Activer GitHub Pages

1. Dans votre dépôt → onglet **Settings**
2. Menu gauche → **Pages**
3. Source → **"GitHub Actions"**
4. Le déploiement se lance automatiquement (1-2 minutes)

### Étape 4 — Accéder à l'application

Votre app sera disponible à :
```
https://VOTRE_USERNAME.github.io/dhl-fleet-management/
```

---

## 📲 Installation sur smartphone

### Android (Chrome)
1. Ouvrir l'URL dans Chrome
2. Une bannière "Installer l'application" apparaît en bas
3. Appuyer sur **📲 Installer**
4. L'icône DHL apparaît sur l'écran d'accueil

### iPhone/iPad (Safari)
1. Ouvrir l'URL dans Safari
2. Appuyer sur l'icône **Partager** (carré avec flèche)
3. Choisir **"Sur l'écran d'accueil"**
4. Appuyer **Ajouter**

### PC (Chrome / Edge)
1. Ouvrir l'URL
2. Cliquer l'icône d'installation dans la barre d'adresse (⊕)
   ou la bannière en bas
3. Cliquer **Installer**

---

## 💾 Données

Les données sont sauvegardées localement dans le navigateur (localStorage).
Elles persistent entre les sessions sur le même appareil.

---

## 🔧 Personnalisation

Pour modifier l'autonomie nominale des camionnettes, éditez `INIT_VANS` dans `index.html`.
