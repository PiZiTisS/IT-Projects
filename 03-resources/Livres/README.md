---
cssclasses:
  - resource-category
status: active
tags:
  - index
  - resource/livre
---

# 📚 Livres - Index

> [!objectif] Objectif
> Centraliser toutes les **notes de lecture, résumés et références** de livres.

---

## 📖 Liste des livres

*Utilise Dataview pour lister automatiquement :*
```dataview
TABLE author, status
FROM "03-resources/Livres"
WHERE file.name != "README"
SORT file.name ASC
```

---

## 🎯 Comment ajouter un livre

> [!etapes] Étapes
> - [ ] Créer une note avec le format : `Auteur - Titre.md` ou `Titre.md`
> - [ ] Utiliser le template **literature-note.md** ou **resource.md**
> - [ ] Remplir les métadonnées : auteur, date, statut
> - [ ] Extraire les idées clés
> - [ ] Lier à des [[02-areas/README|Areas]] ou [[01-projects/README|Projets]] pertinents

---

## 🏷️ Tags recommandés pour les livres

| Tag | Description |
|-----|-------------|
| `#resource/livre` | Catégorie principale |
| `#resource/livre/tech` | Livre technique |
| `#resource/livre/perso` | Livre de développement personnel |
| `#resource/livre/roman` | Roman |
| `#status/a-lire` | À lire |
| `#status/en-cours-lecture` | En train de lire |
| `#status/lu` | Déjà lu |

---

## 📚 Catégories de livres

### 💻 Technologie & Développement
- [[Auteur - Titre 1]]
- [[Auteur - Titre 2]]

### 🧠 Développement Personnel
- [[Auteur - Titre 1]]
- [[Auteur - Titre 2]]

### 📈 Business & Productivité
- [[Auteur - Titre 1]]

### 🎨 Créativité & Design
- [[Auteur - Titre 1]]

---

## 📝 Template pour un livre

Voir : [[templates/literature-note|Template Literature Note]]

---

*Dernière mise à jour : <% tp.date.now("YYYY-MM-DD") %>*
