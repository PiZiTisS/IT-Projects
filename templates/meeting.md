---
cssclasses:
  - meeting
status: en-cours
type: meeting
date: <% tp.date.now("YYYY-MM-DD") %>
participants:
  - <% tp.system.prompt("Participants (séparés par des virgules)") %>
location: <% tp.system.prompt("Lieu/Visio", "Visio") %>
tags:
  - note/meeting
---

# <% tp.file.title %> - Compte-rendu de réunion

> [!info] Métadonnées
> - **Date** : <% tp.file.frontmatter["date"] %>
> - **Heure** : <% tp.system.prompt("Heure", "HH:MM") %>
> - **Lieu** : <% tp.file.frontmatter["location"] %>
> - **Participants** : <% tp.file.frontmatter["participants"] %>

---

## 🎯 Objectifs de la réunion

> [!objectif] But de la réunion
> - Objectif 1
> - Objectif 2

---

## 📋 Ordre du jour

> [!etapes] Points abordés
> - [ ] Point 1
> - [ ] Point 2
> - [ ] Point 3

---

## 📝 Notes et décisions

### 💬 Discussion sur le point 1
[Résumé des échanges]

**Décision :** [Décision prise]
**Responsable :** [Qui fait quoi]
**Échéance :** [Date]

### 💬 Discussion sur le point 2
[Résumé des échanges]

**Décision :** [Décision prise]
**Responsable :** [Qui fait quoi]
**Échéance :** [Date]

---

## ✅ Actions à entreprendre

> [!etapes] Taches issues de la réunion
> - [ ] Tache 1 @[Personne] (échéance : YYYY-MM-DD)
> - [ ] Tache 2 @[Personne] (échéance : YYYY-MM-DD)

---

## 🔗 Liens avec les projets

> [!info] Projets concernés
> - [[Projet 1]]
> - [[Projet 2]]

---

## 📎 Attachments

> [!info] Fichiers joints
> - ![[attachments/2024-11-16-presentations.pdf]]
> - Lien : [Document](URL)

---

## 📝 Prochaines étapes

> [!note] Suivi
> - Prochaine réunion : [[YYYY-MM-DD-Nom]]
> - Points à clarifier :
>   - Point 1
>   - Point 2

---

*Compte-rendu rédigé par : <% tp.user.get("name", "Moi") %>*
