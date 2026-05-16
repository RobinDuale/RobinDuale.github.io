# CLAUDE.md -- Projet projets-duale

Ce fichier guide toutes les conversations dans ce projet. Il est mis à jour au fil des décisions prises.

---

## Contexte du projet

Page d'accueil centrale listant tous les projets GitHub de Robin Duale.
Sert de hub de navigation vers les différents outils et expérimentations publiés.

**URL :** https://projets.duale.fr
**Repo GitHub :** https://github.com/RobinDuale/RobinDuale.github.io
**Chemin local :** `C:\Users\robin\ClaudeDevRepo\projets-duale`
**Branche :** main (déploiement automatique via GitHub Pages)

---

## Stack technique

Site statique HTML pur -- aucun build system, aucun framework.
Tailwind CSS chargé via CDN. Police Inter (Google Fonts).
Déploiement : GitHub Pages, branche main, dossier racine.

---

## Structure du projet

```
projets-duale/
├── CNAME          → projets.duale.fr
├── _redirects     → redirections Netlify (legacy, ne plus utiliser)
├── index.html     → page unique avec toutes les cartes projets
└── CLAUDE.md      → ce fichier
```

## Projets référencés

| Projet | URL | Statut |
|--------|-----|--------|
| Générateur de devis | /devis-generateur/ | Actif |
| Base IA | https://ia.duale.fr | Actif |
| Prochain projet | -- | Placeholder |

---

## Règles absolues

- **Mise à jour de CLAUDE.md en continu** -- ce fichier est la mémoire opérationnelle du projet. L'enrichir dès qu'un nouveau projet est ajouté ou qu'une décision structurante est prise. Ne pas attendre la fin de session.
- **Toujours demander confirmation avant `git push`**
- **Commits en anglais**, co-signés : `Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>`
- **Interdit** : le caractère `—` (tiret cadratin) dans tout contenu créé
- **Noms de fichiers** : minuscules, tirets uniquement

## Démarrage de session -- checklist

1. Lire ce `CLAUDE.md` pour reprendre le contexte
2. `git status` + `git log --oneline -5`
3. Si divergence : `git fetch origin && git reset --hard origin/main`

## Ajout d'un nouveau projet -- procédure

1. Ajouter une carte dans `index.html` en remplacement du bloc "Prochain projet"
2. Remettre un bloc "Prochain projet" après la nouvelle carte
3. Mettre à jour le tableau "Projets référencés" dans ce CLAUDE.md
4. Commit + push (après confirmation)

---

## Historique des décisions

| Date | Decision |
|------|----------|
| 2026-05-16 | Repo cloné en local dans ClaudeDevRepo/projets-duale |
| 2026-05-16 | Carte Base IA ajoutée (ia.duale.fr) |
| 2026-05-16 | Bloc "Prochain projet" conservé comme placeholder permanent |
