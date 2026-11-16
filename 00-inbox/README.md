---
cssclasses:
  - inbox-index
status: active
year: 2024
tags:
  - index
  - inbox
---

# 📥 Inbox - Index

> [!objectif] Objectif
> Capturer rapidement toutes les idées, notes temporaires, liens intéressants et informations à traiter. Ce dossier sert de boîte de réception avant le tri et l'organisation.

---

## 📝 Comment utiliser l'Inbox

### ➕ Ajouter une note
1. Crée une nouvelle note avec le format : `YYYY-MM-DD-Description.md`
2. Utilise le template **Fleeting Note** si disponible
3. Ajoute des tags pour faciliter le tri : `#fleeting`, `#idee`, `#lien`, `#todo`

### 🗂️ Processus de tri (hebdomadaire)

> [!etapes] Étapes de traitement
> - [ ] **Lire** chaque note dans l'inbox
> - [ ] **Classer** :
>   - 🗑️ Supprimer si inutile
>   - 📚 Déplacer vers [[03-resources/README|Resources]] si référence/knowledge
>   - 🎯 Déplacer vers [[02-areas/README|Areas]] si domaine permanent
>   - 🚀 Déplacer vers [[01-projects/README|Projects]] si action concrète
>   - 📅 Déplacer vers [[journal/README|Journal]] si réflexion personnelle
> - [ ] **Lier** la note à d'autres notes existantes

---

## 📋 Notes en attente de tri

*Utilise Dataview pour lister automatiquement :*
```dataview
LIST
FROM "00-inbox"
WHERE file.name != "README"
SORT file.ctime DESC
```

*Ou manuellement :*
- [[2024-11-16-idee-projet]]

---

## 🎯 Bonnes pratiques

> [!tip] Conseils
> - **Ne pas organiser immédiatement** : Capture d'abord, trie plus tard
> - **Garder l'inbox vide** : Traiter régulièrement (quotidien ou hebdo)
> - **Une note = une idée** : Éviter les notes trop longues
> - **Utiliser des liens** : Même dans l'inbox, lie les notes entre elles

> [!warning] À éviter
> - Laisser des notes plus de 7 jours sans tri
> - Créer des sous-dossiers dans l'inbox
> - Stock des notes permanentement ici

---

## 📚 Ressources liées

- [[01-projects/README|Index Projets]]
- [[02-areas/README|Index Areas]]
- [[03-resources/README|Index Resources]]
- [[journal/README|Index Journal]]

---

*Dernière mise à jour : <% tp.date.now("YYYY-MM-DD") %>*
