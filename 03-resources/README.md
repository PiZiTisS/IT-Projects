---
cssclasses:
  - resources-index
status: active
year: 2024
tags:
  - index
  - resource
---

# 📚 Resources - Index

> [!objectif] Objectif
> Centraliser toutes les **connaissances, références, documents et contacts** utiles pour mes projets et mes Areas. Ce sont des informations de valeur à long terme.

---

## 📁 Catégories de Resources

### 📖 Livres & Publications
*Livres, ebooks, articles, papers*
```dataview
LIST
FROM "03-resources/Livres"
WHERE file.name != "README"
SORT file.name ASC
```

### 🎓 Cours & Formations
*Cours en ligne, certifications, tutoriels*
```dataview
LIST
FROM "03-resources/Cours-Formations"
WHERE file.name != "README"
```

### 👥 Contacts
*Personnes, équipes, organisations*
```dataview
LIST
FROM "03-resources/Contacts"
WHERE file.name != "README"
```

### 🛠️ Outils & Logiciels
*Logiciels, applications, services*
```dataview
LIST
FROM "03-resources/Outils-Logiciels"
WHERE file.name != "README"
```

### 📰 Articles & Blogs
*Articles de blog, newsletters*
```dataview
LIST
FROM "03-resources/Articles-Blogs"
WHERE file.name != "README"
```

### 💡 Inspirations
*Citations, idées, concepts*
```dataview
LIST
FROM "03-resources/Inspirations"
WHERE file.name != "README"
```

---

## 🎯 Comment ajouter une Resource

> [!etapes] Étapes
> - [ ] Choisir la catégorie appropriée (ou en créer une nouvelle)
> - [ ] Créer une note avec le format : `Nom-Description.md`
> - [ ] Utiliser le template **resource.md** (si disponible)
> - [ ] Ajouter des métadonnées : auteur, date, source, tags
> - [ ] Extraire les idées clés et notes personnelles
> - [ ] Lier à des [[01-projects/README|Projets]] ou [[02-areas/README|Areas]] pertinents

---

## 🏷️ Système de Tags pour Resources

Voir la documentation complète : [[Tags]]

| Type | Tag | Exemple |
|------|-----|---------|
| Catégorie | `#resource/livre` | `#resource/livre` |
| Type | `#resource/cours` | `#resource/cours/udemy` |
| Domaine | `#domain/tech` | `#domain/developpement` |
| Statut | `#status/a-lire` | `#status/en-cours` |

---

## 📝 Template pour une Resource

```markdown
---
cssclasses:
  - resource
status: a-lire
type: livre
author: [Auteur]
date: [YYYY-MM-DD]
source: [URL ou référence]
tags:
  - resource/livre
  - domain/[domaine]
---

# Titre de la Resource

> [!info] Métadonnées
> - **Auteur** : [Nom]
> - **Date** : [YYYY-MM-DD]
> - **Source** : [Lien ou référence]
> - **Type** : #resource/[type]

## 📖 Résumé
[Résumé en 2-3 paragraphes]

## 💡 Idées clés
- Idée 1
- Idée 2
- Idée 3

## 🔗 Liens avec mes notes
- [[Lien vers projet ou area]]
- [[Autre note liée]]

## 📝 Notes personnelles
[Mes réflexions, applications concrètes, etc.]

## ⭐ Évaluation
- Note : ⭐⭐⭐⭐⭐
- Recommandation : [Oui/Non/Peut-être]
```

---

## 🔍 Recherche dans les Resources

*Utilise Dataview pour des requêtes avancées :*

**Trouver toutes les ressources sur le développement :**
```dataview
LIST
FROM "03-resources"
WHERE contains(tags, "domain/developpement")
```

**Trouver les ressources à lire :**
```dataview
LIST
FROM "03-resources"
WHERE status = "a-lire"
```

---

## 📚 Ressources liées

- [[01-projects/README|Projets]] - Projets utilisant ces resources
- [[02-areas/README|Areas]] - Domaines concernés
- [[Tags|Système de Tags]] - Taxonomie complète

---

*Dernière mise à jour : <% tp.date.now("YYYY-MM-DD") %>*
