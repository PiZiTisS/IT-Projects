---
cssclasses:
  - person
status: active
type: person
relation: <% tp.system.suggester(["collegue", "ami", "famille", "mentor", "contact-pro", "autre"], ["collegue"]) %>
met-date: <% tp.date.now("YYYY-MM-DD") %>
tags:
  - resource/contact
  - person/<% tp.file.title %>
---

# <% tp.file.title %> - Contact

> [!info] Informations de base
> - **Nom complet** : <% tp.system.prompt("Nom complet", tp.file.title) %>
> - **Relation** : #relation/<% tp.file.frontmatter["relation"] %>
> - **Date de rencontre** : <% tp.file.frontmatter["met-date"] %>

---

## 📋 Coordonnées

> [!info] Contacts
> - **Email** : <% tp.system.prompt("Email", "") %>
> - **Téléphone** : <% tp.system.prompt("Téléphone", "") %>
> - **Site web** : [Lien](<% tp.system.prompt("Site web", "") %>)<%-*
> - **LinkedIn** : [Profil](<% tp.system.prompt("LinkedIn", "") %>)<%-*
> - **Twitter** : [@username](<% tp.system.prompt("Twitter", "") %>)<%-*
> - **Adresse** : <% tp.system.prompt("Adresse", "") %>

---

## 💼 Informations professionnelles

> [!info] Carrière
> - **Poste** : <% tp.system.prompt("Poste", "") %>
> - **Entreprise** : <% tp.system.prompt("Entreprise", "") %>
> - **Secteur** : <% tp.system.prompt("Secteur", "") %>
> - **Compétences** :
>   - Compétence 1
>   - Compétence 2

---

## 👤 Informations personnelles

> [!info] Personnel
> - **Date de naissance** : <% tp.system.prompt("Date de naissance", "") %>
> - **Ville** : <% tp.system.prompt("Ville", "") %>
> - **Centres d'intérêt** :
>   - Intérêt 1
>   - Intérêt 2

---

## 📅 Historique des interactions

> [!timeline] Chronologie
> - <% tp.date.now("YYYY-MM-DD") %> : Première rencontre / Note initiale
> - [Date] : [Description de l'interaction]

---

## 💡 Notes et observations

[Mes impressions, choses à retenir, sujets de conversation, etc.]

---

## 🔗 Liens avec mes notes

> [!info] Connexions
> - [[Projet 1]] - Projet en commun
> - [[Resource 1]] - Resource mentionnée par cette personne
> - [[Note personnelle]] - Réflexion liée

---

## 📝 Prochaines actions

> [!etapes] Suivi
> - [ ] Prendre contact pour [raison] (échéance : YYYY-MM-DD)
> - [ ] Envoyer [document/email] (échéance : YYYY-MM-DD)
> - [ ] Organiser une réunion (échéance : YYYY-MM-DD)

---

## ⭐ Importance

> [!note] Évaluation
> - **Niveau de relation** : ⭐⭐⭐⭐⭐
> - **Utilité** : Haute / Moyenne / Faible
> - **Fréquence de contact** : Quotidienne / Hebdomadaire / Mensuelle / Rare
