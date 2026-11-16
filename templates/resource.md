---
cssclasses:
  - resource
status: a-lire
type: <% tp.system.suggester(["livre", "cours", "article", "video", "podcast", "outil", "document", "contact"], ["livre"]) %>
author: <% tp.system.prompt("Auteur") %>
date: <% tp.date.now("YYYY-MM-DD") %>
source: <% tp.system.prompt("Source/URL") %>
tags:
  - resource/<% tp.file.basename %>
---

# <% tp.file.title %>

> [!info] Métadonnées
> - **Type** : #resource/<% tp.file.basename %>
> - **Auteur** : <% tp.file.frontmatter["author"] %>
> - **Date** : <% tp.file.frontmatter["date"] %>
> - **Source** : [Lien](<% tp.file.frontmatter["source"] %>)<%-*
> - **Statut** : #status/<% tp.file.frontmatter["status"] %>

---

## 📖 Résumé

[Résumé en 2-3 paragraphes de la resource]

---

## 💡 Idées clés

> [!etapes] Principaux enseignements
> - [ ] Idée ou concept 1
> - [ ] Idée ou concept 2
> - [ ] Idée ou concept 3

---

## 📝 Notes personnelles

[Mes réflexions, applications concrètes, questions, etc.]

---

## 🔗 Liens avec mes notes

> [!info] Notes liées
> - [[Note 1]]
> - [[Note 2]]
> - [[Projet associé]]

---

## ⭐ Évaluation

> [!note] Mon avis
> - **Note** : ⭐⭐⭐⭐⭐
> - **Recommandation** : Oui / Non / Peut-être
> - **À revoir** : Oui / Non

---

## 🎯 Actions à entreprendre

> [!etapes] Prochaines étapes
> - [ ] Action 1
> - [ ] Action 2
