# ⚽ FootGuessr

Jeu de devinette football. Devine le joueur grâce à 3 indices : nationalité, poste, club & période.
197 joueurs couvrant toutes les époques, de Pelé à Lamine Yamal.

**Zéro API, zéro backend, zéro coût.** Les joueurs sont dans `players.json`.

---

## 🚀 Déploiement (5 minutes)

### 1. Mets le projet sur GitHub
```bash
git init
git add .
git commit -m "Initial commit - FootGuessr"
# Crée un repo sur github.com puis :
git remote add origin https://github.com/TON_USERNAME/footguessr.git
git push -u origin main
```

### 2. Déploie sur Vercel (ou Netlify ou GitHub Pages)
- Va sur https://vercel.com → connecte-toi avec GitHub
- "Add New Project" → sélectionne `footguessr` → Deploy
- C'est tout. Aucune variable d'environnement nécessaire.

### 3. Installe sur ton téléphone
**Android (Chrome) :** Menu ⋮ → "Ajouter à l'écran d'accueil"
**iPhone (Safari) :** Bouton partage → "Sur l'écran d'accueil"

---

## 📁 Structure

```
footguessr/
├── index.html      ← Le jeu complet
├── players.json    ← Base de données des 197 joueurs
├── manifest.json   ← Config PWA
├── sw.js           ← Mode hors-ligne
└── icons/
    ├── icon-192.png
    └── icon-512.png
```

## ➕ Ajouter des joueurs

Édite `players.json` en suivant ce format :
```json
{
  "name": "Zinedine Zidane",
  "country": "France 🇫🇷",
  "position": "Milieu offensif",
  "club": "Real Madrid (2001–2006)",
  "era": "2000s",
  "answers": ["zinedine zidane", "zidane", "zizou"]
}
```
Valeurs possibles pour `era` : `classic`, `80s`, `90s`, `2000s`, `2010s`, `2020s`
