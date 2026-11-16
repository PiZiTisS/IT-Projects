---
cssclasses:
  - archive-category
status: active
tags:
  - index
  - archive
---

# 📄 Notes Archivées - Index

> [!objectif] Objectif
> Stocker les **notes obsolètes ou temporaires** qui ne sont plus pertinentes mais qu'on souhaite conserver.

---

## 📝 Types de notes archivées

| Type | Description | Exemple |
|------|-------------|---------|
| Fleeting Notes | Notes temporaires traitées | `2024-01-15-idee-rapide.md` |
| Notes obsolètes | Informations dépassées | `Ancien-Projet-Specifications.md` |
| Versions précédentes | Anciennes versions de notes | `Projet-V1.md` |

---

## 📋 Liste des notes archivées

*Utilise Dataview pour lister automatiquement :*
```dataview
LIST
FROM "04-archive/Notes-Archivees"
WHERE file.name != "README"
SORT file.ctime DESC
```

---

## 🎯 Quand archiver une note ?

> [!etapes] Critères
> - [ ] Note de type **fleeting** traitée et classée ailleurs
> - [ ] Note avec des **informations obsolètes**
> - [ ] **Ancienne version** d'une note mise à jour
> - [ ] Note **non liée** à d'autres notes depuis plus de 6 mois

---

## ⚠️ Attention

> [!warning] Avant d'archiver
> - Vérifier que la note n'est **référencée nulle part** (utiliser le graphe ou backlinks)
> - Conserver une **copie de sauvegarde** si la note est importante
> - Ne pas archiver les **notes permanentes** (permanent notes)

---

## 📚 Ressources liées

- [[04-archive/README|Retour à l'archive principale]]
- [[00-inbox/README|Inbox]] - Pour les nouvelles notes temporaires

---

*Dernière mise à jour : <% tp.date.now("YYYY-MM-DD") %>*
