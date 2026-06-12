# 📱 Installer « Mondial 2026 » sur Android

L'app est une **PWA** (Progressive Web App). Pour l'installer sur ton téléphone,
il faut la mettre en ligne en HTTPS (gratuit, 2 minutes), puis l'ajouter à l'écran d'accueil.

## Fichiers à mettre en ligne
Mets **tout le contenu** de ce dossier *sauf* `.claude/`, `INSTALL-ANDROID.md` et `*.py` :

- `index.html`
- `manifest.webmanifest`
- `sw.js`
- `icon-192.png`
- `icon-512.png`
- `apple-touch-icon.png`

## Option A — Netlify Drop (le plus simple, sans compte)
1. Sur ton PC, va sur **https://app.netlify.com/drop**
2. **Glisse-dépose** le dossier (ou les fichiers listés ci-dessus) dans la zone.
3. Netlify te donne une **URL en https://…netlify.app** → c'est ton app en ligne.
   *(Crée un compte gratuit pour que l'URL reste permanente.)*

## Option B — GitHub Pages
1. Crée un dépôt GitHub, ajoute-y les fichiers.
2. Settings → Pages → Branch `main` /root → Save.
3. Ton app sera sur `https://<utilisateur>.github.io/<dépôt>/`.

## Installer sur le téléphone
1. Ouvre l'URL https dans **Chrome sur Android**.
2. Soit tu tapes le bouton vert **« ⬇️ Installer l'application »**,
   soit le menu **⋮ → « Installer l'application »** / « Ajouter à l'écran d'accueil ».
3. Une icône ⚽ apparaît sur ton écran d'accueil → elle s'ouvre en plein écran, comme une vraie app.

## Ce qui marche hors-ligne
- L'app, les matchs, tes notes, ton statut de visionnage et tes pronostics : **oui** (tout est local).
- Les drapeaux : mis en cache après la 1ʳᵉ ouverture.
- Les **scores en direct** : nécessitent internet (sinon, dernier état connu).

## Mettre à jour l'app plus tard
Si tu modifies `index.html`, change aussi la ligne `const CACHE = "wc2026-v1"`
dans `sw.js` (ex. `"wc2026-v2"`) puis re-héberge : le téléphone récupérera la nouvelle version.
