---
cssclasses:
  - resource-category
status: active
tags:
  - index
  - resource/contact
---

# 👥 Contacts - Index

> [!objectif] Objectif
> Gérer et organiser les **contacts professionnels et personnels** avec leurs informations et l'historique des interactions.

---

## 📋 Liste des contacts

*Utilise Dataview pour lister automatiquement :*
```dataview
TABLE relation, met-date
FROM "03-resources/Contacts"
WHERE file.name != "README"
SORT met-date DESC
```

---

## 🎯 Comment ajouter un contact

> [!etapes] Étapes
> - [ ] Créer une note avec le format : `Prenom-Nom.md`
> - [ ] Utiliser le template **person.md**
> - [ ] Remplir les informations de base (coordonnées, relation)
> - [ ] Ajouter des notes sur les interactions
> - [ ] Lier à des [[01-projects/README|Projets]] ou [[02-areas/README|Areas]] communs

---

## 👤 Catégories de contacts

### 💼 Professionnels
- [[Prenom-Nom]] - Poste, Entreprise

### 👨‍👩‍👧‍👦 Personnel
- [[Prenom-Nom]] - Relation

### 🎓 Mentors & Conseillers
- [[Prenom-Nom]] - Domaine d'expertise

---

## 🏷️ Tags recommandés pour les contacts

| Tag | Description |
|-----|-------------|
| `#resource/contact` | Catégorie principale |
| `#relation/collegue` | Collègue de travail |
| `#relation/ami` | Ami |
| `#relation/famille` | Membre de la famille |
| `#relation/mentor` | Mentor |
| `#relation/client` | Client |
| `#relation/fournisseur` | Fournisseur |

---

## 📅 Suivi des contacts

### ⚠️ Contacts à recontacter
```dataview
LIST
FROM "03-resources/Contacts"
WHERE contains(file.tasks, "[ ] Prendre contact")
```

### 📅 Prochains anniversaires
*À implémenter avec Dataview ou un plugin de calendrier*

---

## 💡 Bonnes pratiques

> [!tip] Conseils
> - **Mettre à jour régulièrement** les informations de contact
> - **Noter les interactions** importantes après chaque échange
> - **Créer des rappels** pour les anniversaires et dates importantes
> - **Organiser par relation** plutôt que par nom

---

## 📚 Ressources liées

- [[templates/person|Template Person]]
- [[01-projects/README|Projets]] - Projets impliquant ces contacts

---

*Dernière mise à jour : <% tp.date.now("YYYY-MM-DD") %>*
