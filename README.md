# Workshop DORA interactif

> Mettre en pratique le cours en **prenant des décisions d'architecture**, pas en récitant des API.
> Public : technique mixte (dev, DevOps/Cloud, sécurité, data, architectes). Aucune connaissance d'une API Python requise.

## Objectif

À travers un cas unique — l'assistant de conformité DORA — chaque équipe conçoit, sécurise et optimise une plateforme IA. On raisonne toujours :

```
Problème métier → risque technique → solution architecturale → techno → compromis
```

## Modalités pédagogiques

Les **69 exercices sont obligatoires pour tous les apprenants**. Ils sont répartis sur plusieurs séquences ; seule la profondeur de réponse évolue de N1 à N4.

| Modalité | Organisation |
| --- | --- |
| Séquence guidée | Un bloc thématique, sa correction et l'active recall associée |
| Travail autonome | Réponse individuelle N1/N2, puis comparaison avec le corrigé |
| Travail en équipe | Production N2/N3 et justification des compromis |
| Cycle complet | Tous les niveaux et tous les exercices, avec le projet DORA comme fil rouge |

## Les cinq niveaux

| Niveau | Finalité | Exercices |
| --- | --- | ---: |
| 1. Fondamentaux | Comprendre LLM, génération et vocabulaire | 0–0 bis |
| 2. Architecture cœur | Choisir frameworks, mémoire, sécurité et coût | 1–7 + bonus |
| 3. Enterprise engineering | Adapter, évaluer, gouverner et livrer | 8–35 |
| 4. Spécialisations | Prompt, contexte, modèles, RAG, agents, MCP, safety, observabilité et évaluation | 36–65 |
| 5. Production mastery | Admission, files, scaling, fiabilité et incidents | 66–68 |

## Progression commune obligatoire

| Phase | Exercices | Résultat attendu |
| --- | ---: | --- |
| Fondations | 0–13 | Expliquer les concepts et prendre une première décision justifiée |
| Architecture entreprise | 14–35 | Concevoir le système DORA complet et ses contrôles |
| Spécialisations | 36–65 | Approfondir chaque composant sans perdre la vision système |
| Production | 66–68 | Exploiter, fiabiliser et gérer les incidents |
| Synthèse | 0–68 | Relier toutes les décisions dans une architecture finale défendable |

## Règles du jeu

- Chaque réponse doit nommer **le besoin/capacité** avant la techno.
- Justifier aussi **pourquoi pas les autres options**.
- Il n'y a pas toujours une seule bonne réponse : le raisonnement compte autant que le choix.

## Le cas fil rouge

> *« Analyse ce contrat fournisseur et dis-moi s'il présente un risque DORA. »*

Le système doit : récupérer le contrat depuis SharePoint → extraire le texte → chercher les exigences DORA pertinentes → analyser → si confiance faible, demander une validation humaine → sinon générer le rapport → enregistrer en base → pouvoir reprendre après interruption.

## Fichiers

- [`01-exercices.md`](01-exercices.md) — énoncés (version participants, sans réponses)
- `02-corrige.md` — corrigés + raisonnement (version animateur) — *non publié*
- `03-active-recall.md` — checklist d'auto-évaluation — *non publié*

> **Note `.gitignore`** : `02-corrige.md` et `03-active-recall.md` sont volontairement exclus du dépôt (listés dans `.gitignore`). Ce sont des supports animateur qui ne doivent pas être partagés avec les participants.

Le fichier participants commence par une **carte des 25 blocs thématiques** et se termine par des **références officielles pour les étudiants** (Ragas, DeepEval, Langfuse, Helicone et MCP). Les mêmes regroupements sont repris dans le corrigé animateur. Les numéros d'exercices restent stables pour permettre les renvois entre supports.
