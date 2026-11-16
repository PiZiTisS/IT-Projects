---
cssclasses:
  - archive-index
status: active
year: 2024
tags:
  - index
  - archive
---

# 🗃️ Archive - Index

> [!objectif] Objectif
> Stocker les **projets terminés, notes obsolètes et archives** pour garder le vault propre et organisé tout en conservant l'historique.

---

## 📁 Structure de l'Archive

### 🗂️ Projets archivés
*Projets terminés ou abandonnés*
```dataview
LIST
FROM "04-archive/Projets-Termines"
SORT file.name DESC
```

### 📄 Notes archivées
*Notes obsolètes ou non pertinentes*
```dataview
LIST
FROM "04-archive/Notes-Archivees"
SORT file.name DESC
```

---

## 🎯 Quand archiver ?

> [!etapes] Critères d'archivage
> - [ ] **Projets** : Statut `termine` ou `abandonne` depuis plus de 3 mois
> - [ ] **Notes temporaires** : Notes de type `fleeting` traitées
> - [ ] **Resources obsolètes** : Informations dépassées ou inutiles
> - [ ] **Anciennes versions** : Versions précédentes de notes importantes

---

## 📝 Comment archiver ?

> [!etapes] Processus d'archivage
> - [ ] Vérifier que le projet/note est **vraiment terminé**
> - [ ] Créer un **rapport final** si nécessaire (pour les projets)
> - [ ] Déplacer vers le dossier approprié :
>   - `04-archive/Projets-Termines/YYYY/` pour les projets
>   - `04-archive/Notes-Archivees/` pour les notes
> - [ ] Ajouter le tag `#archive/YYYY`
> - [ ] Mettre à jour les **liens** dans le vault (si nécessaire)
> - [ ] Noter dans le **journal** : "Archivé [nom] le [date]"

---

## 📋 Template pour l'archivage d'un projet

```markdown
---
cssclasses:
  - archive
status: termine
archive-date: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - project/NOM
  - archive/<% tp.date.now("YYYY") %>
---

# [NOM] - Archive

> [!info] Informations d'archivage
> - **Date d'archivage** : <% tp.date.now("YYYY-MM-DD") %>
> - **Statut final** : termine/abandonne
> - **Durée** : [YYYY-MM-DD] → <% tp.date.now("YYYY-MM-DD") %>

## 📖 Résumé du projet
[Résumé des objectifs et résultats]

## ✅ Résultats obtenus
- Résultat 1
- Résultat 2
- Résultat 3

## 📚 Ressources produites
- [[Lien vers resource 1]]
- [[Lien vers resource 2]]

## 💡 Leçons apprises
- Leçon 1
- Leçon 2
- Leçon 3

## 🔗 Liens archivés
- [Lien 1](url)
- [Lien 2](url)
```

---

## 🔍 Recherche dans l'Archive

*Utilise Dataview pour explorer l'archive :*

**Trouver tous les projets archivés en 2024 :**
```dataview
LIST
FROM "04-archive/Projets-Termines/2024"
```

**Trouver les projets terminés :**
```dataview
LIST
FROM "04-archive"
WHERE status = "termine"
```

---

## 🗑️ Nettoyage de l'Archive

> [!todo] Taches de maintenance
> - [ ] **Tous les 6 mois** : Vérifier et supprimer les notes inutiles
> - [ ] **Tous les ans** : Compresser les anciennes archives (zip)
> - [ ] **Tous les ans** : Mettre à jour les liens cassés

---

## 📚 Ressources liées

- [[01-projects/README|Projets]] - Projets actifs
- [[02-areas/README|Areas]] - Domaines de responsabilité
- [[03-resources/README|Resources]] - Connaissances archivées
- [[journal/README|Journal]] - Historique des actions

---

*Dernière mise à jour : <% tp.date.now("YYYY-MM-DD") %>*
