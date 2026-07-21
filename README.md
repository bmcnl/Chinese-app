# 中文 — Apprendre le mandarin (PWA)

Application web progressive (PWA) pour apprendre le mandarin :
vocabulaire avec audio, grammaire, dialogues, exercices. Version de
départ : 6 unités de niveau débutant (tons/pinyin, pronoms, nombres,
classificateurs, particules de phrase, restaurant).

## Contenu du package

```
.
├── index.html          → l'application (tout le contenu est ici)
├── manifest.json        → métadonnées PWA (nom, icônes, couleurs)
├── sw.js                 → service worker (cache hors-ligne)
├── icons/
│   ├── icon-192.png
│   ├── icon-512.png
│   └── icon-maskable-512.png
└── README.md             → ce fichier
```

Fichiers statiques, aucune étape de build nécessaire.

---

## 1. Mettre le projet sur GitHub

1. Va sur [github.com/new](https://github.com/new).
2. Nom du dépôt, par exemple `zhongwen-mandarin`. Laisse-le **Public**,
   ne coche aucune case d'initialisation.
3. Clique sur **Create repository**.
4. Dans le dossier contenant `index.html` :

   ```bash
   git init
   git add .
   git commit -m "Premier envoi du site mandarin"
   git branch -M main
   git remote add origin https://github.com/TON-PSEUDO/zhongwen-mandarin.git
   git push -u origin main
   ```

   (ou glisse-dépose les fichiers directement sur la page GitHub si tu
   préfères éviter la ligne de commande.)

---

## 2. Déployer sur Vercel

1. [vercel.com](https://vercel.com) → connecte-toi avec ton compte GitHub.
2. **Add New... → Project** → choisis `zhongwen-mandarin` → **Import**.
3. Ne change aucun réglage (site 100% statique) → **Deploy**.
4. En ~30 secondes, ton site est en ligne sur une URL du type
   `https://zhongwen-mandarin.vercel.app`.

### Mises à jour futures

```bash
git add .
git commit -m "description du changement"
git push
```
Vercel redéploie automatiquement à chaque push.

### Installer la PWA sur un téléphone

- **Android/Chrome** : ouvrir le lien → menu ⋮ → "Ajouter à l'écran
  d'accueil".
- **iPhone/Safari** : ouvrir le lien → bouton Partager → "Sur l'écran
  d'accueil".

---

## Remarques

- **Caractères** : le site utilise le chinois **simplifié** (norme de
  Chine continentale). Si ta belle-famille ou tes contacts utilisent
  le **traditionnel** (Taïwan, Hong Kong), dis-le-moi : je peux faire
  une bascule ou une double présentation des caractères.
- **Audio** : comme pour le site vietnamien, la prononciation utilise
  la synthèse vocale du navigateur (voix chinoise installée sur
  l'appareil) — pratique pour le rythme et les tons de base, mais ne
  remplace pas l'écoute de vrais locuteurs.
- **Cache/mise à jour du site** : si une modification n'apparaît pas
  immédiatement pour les visiteurs ayant déjà chargé le site, augmente
  le numéro de version en haut de `sw.js` :
  ```js
  const CACHE_NAME = "zhongwen-v2"; // v1 → v2
  ```
