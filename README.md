# ⚽ Coupe du Monde 2026 — Mes notes

Application web (PWA) pour suivre **tous les matchs du Mondial 2026** : noter chaque match,
marquer son statut de visionnage, voir les **scores en direct** et remplir son **pronostic du tableau final**.

## Fonctionnalités
- 104 matchs (phase de groupes + phases finales) avec heure française et diffuseur (M6 / beIN).
- Note par étoiles + commentaire, sauvegardés localement (localStorage).
- Statut de visionnage : Pas vu / Mi-temps / Vu.
- Scores en direct (via l'API gratuite TheSportsDB), rafraîchis automatiquement.
- Page Pronostics : bracket interactif du tableau final.
- Installable sur Android / iOS (PWA, fonctionne hors-ligne).

## Utilisation
Site statique : ouvrir `index.html`. Pour l'installer sur mobile, voir
[INSTALL-ANDROID.md](INSTALL-ANDROID.md).

## Hébergement
Conçu pour GitHub Pages : activer Pages sur la branche `main` (dossier racine).
