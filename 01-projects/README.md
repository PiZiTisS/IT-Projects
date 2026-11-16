---
cssclasses:
  - projects-index
status: active
year: 2024
tags:
  - index
  - project
---

# 🚀 Projets - Index

> [!objectif] Objectif
> Lister et suivre tous les projets actifs avec des objectifs clairs, des échéances et un suivi de progression.

---

## 📋 Projets actifs

*Utilise Dataview pour lister automatiquement :*
```dataview
TABLE status, start, year
FROM "01-projects"
WHERE file.name != "README" AND status != "termine"
SORT start DESC
```

*Ou manuellement :*

### 2026
- [[2026-B1/Projet_test]] - #status/en-cours

---

## 🎯 Comment créer un nouveau projet

> [!etapes] Étapes
> - [ ] Créer un dossier avec le format : `YYYY-Nom-Projet/`
> - [ ] Utiliser le template **projet.md** (via Templater ou manuellement)
> - [ ] Remplir les métadonnées (objectif, statut, tags)
> - [ ] Définir les prochaines étapes concrètes
> - [ ] Lier le projet à une [[02-areas/README|Area]] si applicable
> - [ ] Créer une note dans [[journal/README|Journal]] pour le suivi

---

## 📊 Statuts des projets

| Statut | Description | Icône |
|--------|-------------|-------|
| `en-cours` | Projet actif en développement | 🚀 |
| `en-attente` | Projet planifié mais pas encore démarré | ⏳ |
| `en-pause` | Projet temporairement suspendu | ⏸️ |
| `termine` | Projet achevé (à archiver) | ✅ |
| `abandonne` | Projet annulé | ❌ |

---

## 🗑️ Projets à archiver

> [!todo] À faire
> - [ ] Vérifier les projets avec statut `termine`
> - [ ] Déplacer vers [[04-archive/README|Archive]]
> - [ ] Créer un rapport final si nécessaire

*Requête Dataview :*
```dataview
LIST
FROM "01-projects"
WHERE status = "termine"
```

---

## 📚 Ressources liées

- [[00-inbox/README|Inbox]] - Pour capturer de nouvelles idées de projets
- [[02-areas/README|Areas]] - Domaines de responsabilité associés
- [[03-resources/README|Resources]] - Documents et références utiles
- [[templates/projet|Template Projet]] - Modèle à utiliser

---

*Dernière mise à jour : <% tp.date.now("YYYY-MM-DD") %>*
