---
cssclasses:
  - areas-index
status: active
year: 2024
tags:
  - index
  - area
---

# 🎯 Areas - Index

> [!objectif] Objectif
> Définir et suivre les **domaines de responsabilité permanente** de ma vie. Contrairement aux projets (temporaires), les Areas sont des aspects permanents qui nécessitent une attention continue.

---

## 📋 Mes Areas principales

*Utilise Dataview pour lister automatiquement :*
```dataview
TABLE description, status
FROM "02-areas"
WHERE file.name != "README"
SORT file.name ASC
```

*Structure suggérée :*

### 💼 Professionnel
- [[Developpement-Pro]] - Compétences techniques et évolution de carrière
- [[Veille-Technologique]] - Suivi des tendances et innovations

### 🏡 Personnel
- [[Sante]] - Santé physique et mentale
- [[Finances]] - Gestion budgétaire et investissements
- [[Relations]] - Vie sociale et familiale

### 🎓 Apprentissage
- [[Formation-Continue]] - Cours, certifications, auto-apprentissage
- [[Lecture]] - Livres, articles, ressources éducatives

---

## 🎯 Comment créer une nouvelle Area

> [!etapes] Étapes
> - [ ] Créer un fichier avec le nom de l'Area (sans dossier)
> - [ ] Utiliser le template **area.md** (si disponible)
> - [ ] Définir l'objectif principal de cette Area
> - [ ] Identifier les standards de succès
> - [ ] Lister les actions récurrentes
> - [ ] Associer à des [[01-projects/README|Projets]] si applicable

---

## 📝 Template pour une Area

```markdown
---
cssclasses:
  - area
status: active
tags:
  - area/NOM
---

# NOM

> [!objectif] Objectif principal
> [Décris en une phrase l'objectif de cette Area]

## 🎯 Standards de succès
- [ ] Standard 1
- [ ] Standard 2
- [ ] Standard 3

## 📅 Actions récurrentes
- [ ] Action hebdomadaire
- [ ] Action mensuelle
- [ ] Action trimestrielle

## 🔗 Ressources associées
- [[Lien vers resource 1]]
- [[Lien vers resource 2]]

## 📊 Suivi
- {{date:YYYY-MM-DD}} : [Note sur l'avancement]
```

---

## 🔄 Review des Areas

> [!todo] Review Hebdomadaire
> - [ ] Vérifier l'avancement de chaque Area
> - [ ] Mettre à jour les standards si nécessaire
> - [ ] Planifier les actions pour la semaine

> [!todo] Review Mensuelle
> - [ ] Évaluer les résultats du mois
> - [ ] Ajuster les priorités
> - [ ] Identifier les blocages

---

## 📚 Ressources liées

- [[01-projects/README|Projets]] - Projets associés à ces Areas
- [[03-resources/README|Resources]] - Connaissances pour soutenir ces Areas
- [[00-inbox/README|Inbox]] - Pour capturer de nouvelles idées

---

*Dernière mise à jour : <% tp.date.now("YYYY-MM-DD") %>*
