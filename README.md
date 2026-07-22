# 中文 Zhongwen Mandarin — Progressive Web App

Une application complète et interactive pour apprendre le mandarin chinois.

## 📱 Caractéristiques

- **80 unités** de vocabulaire (HSK 1-6 + Médical + Voyage)
- **900 exercices interactifs** (QCM, écoute, complétion)
- **Grammaire détaillée** pour les niveaux 1-6
- **Dialogues contextuels** pour chaque unité
- **Audio pronunciation** avec synthèse vocale
- **Mot du jour** qui change chaque jour
- **Glossaire compilé** avec 443 mots
- **Traducteur intégré** (DeepL)
- **Barre de progression** pour suivre l'avancement
- **Mode sombre** pour l'étude le soir
- **Installable sur iPhone/Android**
- **Fonctionne hors ligne**

## 🚀 Déploiement

### Fichiers nécessaires

```
zhongwen-mandarin.html     # Application principale
manifest.json              # Métadonnées PWA
sw.js                      # Service worker (offline)
icon-192.png              # Icône 192x192
icon-512.png              # Icône 512x512
icon-maskable-192.png     # Icône adaptative 192x192
icon-maskable-512.png     # Icône adaptative 512x512
README.md                 # Ce fichier
```

### Sur GitHub Pages

1. **Crée un repository** `zhongwen-mandarin` sur GitHub
2. **Upload les fichiers** listés ci-dessus
3. Va dans **Settings → Pages**
4. Sélectionne **Branch: main** et clique **Save**
5. Ton app est live! 🎉

URL: `https://[ton-username].github.io/zhongwen-mandarin/`

### Sur Vercel

1. Connecte ton repo GitHub à Vercel
2. Selectionne `zhongwen-mandarin`
3. Clique **Import** — c'est déployé! 🚀

URL: `https://zhongwen-mandarin.vercel.app/`

## 📲 Installation sur iPhone

1. Ouvre l'app dans Safari
2. Clique le bouton **Partage** (carré avec flèche)
3. Sélectionne **"Ajouter à l'écran d'accueil"**
4. Confirme — l'app s'installe! ✅

## 📲 Installation sur Android

1. Ouvre l'app dans Chrome
2. Clique les **3 points** (menu)
3. Sélectionne **"Installer l'app"**
4. Confirme — l'app s'installe! ✅

## 🌐 Fonctionnalités hors ligne

- Tous les contenus (vocabulaire, exercices, dialogues) sont **disponibles offline**
- Le mode sombre et tes **préférences sont sauvegardées** localement
- Parfait pour étudier en transport ou en voyage ✈️

## 🛠 Personnalisation

### Modifier les icônes

Les icônes actuelles sont simples. Tu peux les remplacer par:
- Un logo personnalisé (192x192 et 512x512 PNG)
- Les garder telles quelles ✅

### Modifier la couleur du thème

Édite `manifest.json`:
```json
"theme_color": "#B7282E",        // Couleur barre en haut
"background_color": "#F3EFE6"   // Couleur écran de démarrage
```

## 📊 Structure de l'app

### Niveaux

- **HSK 1-6**: Curriculum officiel chinois
- **Niveau 7**: Vocabulaire médical (10 unités)
- **Niveau 8**: Vocabulaire complet + voyage (10 unités)

### Types d'exercices

1. **QCM** — Choix multiple (5 par unité)
2. **Écoute** — Prononciation (5 par unité)
3. **Complétion** — Remplissage pinyin (5 par unité)

Score requis: **≥60%** pour valider une unité.

## 🎯 Conseils d'utilisation

- 📅 Consulte le **Mot du jour** chaque matin
- 📖 Utilise le **Glossaire** pour réviser
- 🎤 Écoute la **prononciation** plusieurs fois
- 🌙 Passe en **mode sombre** le soir
- 📊 Suis ta **progression** pour rester motivé

## 🔧 Support technique

Si l'app ne se charge pas:
1. Vide le cache du navigateur
2. Désenregistre le service worker (DevTools → Application → Unregister)
3. Recharge la page

Si le traducteur ne fonctionne pas:
- Vérifie ta connexion internet (offline OK pour le reste)
- DeepL fonctionne mieux avec Chrome/Safari

## 📝 Changelog

### v1.0.0 (Juillet 2026)
- ✅ 80 unités complètes
- ✅ 900 exercices
- ✅ PWA installable
- ✅ Mode sombre
- ✅ Offline support

---

**Bon apprentissage!** 加油! (jiāyóu!)

Faite avec ❤️ pour les apprenants du mandarin
