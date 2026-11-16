---
cssclasses:
  - archive-category
status: active
tags:
  - index
  - archive
---

# 🗂️ Projets Terminés - Index

> [!objectif] Objectif
> Archiver les **projets achevés** par année pour conserver l'historique tout en gardant le vault organisé.

---

## 📁 Projets par année

### 2024
```dataview
LIST
FROM "04-archive/Projets-Termines/2024"
SORT file.name ASC
```

### 2025
```dataview
LIST
FROM "04-archive/Projets-Termines/2025"
SORT file.name ASC
```

---

## 🎯 Comment archiver un projet

> [!etapes] Processus
> - [ ] Vérifier que le projet est **vraiment terminé**
> - [ ] Créer un **rapport final** dans le dossier du projet
> - [ ] Déplacer le dossier du projet vers `04-archive/Projets-Termines/YYYY/`
> - [ ] Mettre à jour le statut : `#status/termine`
> - [ ] Ajouter le tag : `#archive/YYYY`
> - [ ] Noter dans le [[journal/README|journal]] : "Archivé [nom] le [date]"

---

## 📚 Ressources liées

- [[04-archive/README|Retour à l'archive principale]]
- [[01-projects/README|Projets actifs]]

---

*Dernière mise à jour : <% tp.date.now("YYYY-MM-DD") %>*
