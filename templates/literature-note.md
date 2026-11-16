---
cssclasses:
  - literature-note
status: en-cours
type: literature-note
source: <% tp.system.prompt("Titre de la source") %>
author: <% tp.system.prompt("Auteur") %>
pages: <% tp.system.prompt("Nombre de pages", "0") %>
read-date: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - note/litterature
  - resource/<% tp.system.suggester(["livre", "article", "paper", "blog"], ["livre"]) %>
---

# <% tp.file.title %> - Note de lecture

> [!info] Métadonnées
> - **Source** : <% tp.file.frontmatter["source"] %>
> - **Auteur** : <% tp.file.frontmatter["author"] %>
> - **Pages** : <% tp.file.frontmatter["pages"] %>
> - **Date de lecture** : <% tp.file.frontmatter["read-date"] %>

---

## 📖 Résumé global

[Résumé en 1-2 paragraphes du contenu principal]

---

## 💡 Points clés et citations

> [!quote] Citation 1
> > "Citation importante"
> — Auteur, Page XX

> [!quote] Citation 2
> > "Autre citation"
> — Auteur, Page YY

---

## 📝 Mes réflexions

[Mes pensées, questions, connexions avec mes propres connaissances]

---

## 🔗 Connexions avec mes notes

> [!info] Notes existantes liées
> - [[Note connexe 1]] - Explication de la connexion
> - [[Note connexe 2]] - Explication de la connexion

---

## 🎯 Applications pratiques

> [!etapes] Comment appliquer ces idées
> - [ ] Application 1
> - [ ] Application 2

---

## ⭐ Évaluation

> [!note] Mon avis
> - **Note** : ⭐⭐⭐⭐⭐
> - **Pertinence** : Haute / Moyenne / Faible
> - **À relire** : Oui / Non

---

## 🏷️ Tags supplémentaires

[Ajouter des tags spécifiques au contenu]
