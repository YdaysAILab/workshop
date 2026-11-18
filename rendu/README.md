# Rendu des étudiant·e·s

> ⏰ **Date limite : 25.11.2026 à 23h59.**

Chaque étudiant·e dépose **son rendu** ici, dans ce dossier `rendu/`.

## Règles

1. **Un seul fichier Markdown (`.md`) par étudiant·e.**
2. **Nom du fichier = prénom et nom**, en minuscules, sans accents ni espaces (kebab-case) : `prenom-nom.md`.
   - *Jean Dupont* → `jean-dupont.md`
   - *Amélie Kanmegné* → `amelie-kanmegne.md`
3. **Travaille sur ta propre branche** — jamais directement sur `main`.
4. Dépose ton fichier dans `rendu/`, pousse ta branche, puis ouvre une **Pull Request** vers `main`.

## Marche à suivre (copier-coller)

```bash
git checkout main && git pull
git checkout -b rendu/prenom-nom
# crée rendu/prenom-nom.md et réponds aux exercices
git add rendu/prenom-nom.md
git commit -m "Rendu — Prénom Nom"
git push -u origin rendu/prenom-nom
# puis ouvre une Pull Request sur GitHub vers main
```

## Modèle de fichier

~~~markdown
# Rendu — Prénom Nom

> Workshop DORA — <date>

## Exercice N — <titre>
**Besoin / capacité :** …
**Choix :** …
**Pourquoi pas les autres options :** …
**Compromis :** …
~~~
