---
cssclasses:
  - journal-index
status: active
year: 2024
tags:
  - index
  - journal
---

# 📅 Journal - Index

> [!objectif] Objectif
> **Centraliser les notes quotidiennes, réflexions et suivis** pour créer une trace chronologique de mes pensées, actions et apprentissages.

---

## 📅 Structure du Journal

```
journal/
├── 2024/
│   ├── 2024-11/
│   │   ├── 2024-11-16.md
│   │   ├── 2024-11-17.md
│   │   └── ...
│   └── 2024-12/
│       └── ...
└── 2025/
    └── ...
```

---

## 📝 Types de notes dans le Journal

| Type | Description | Template | Tags |
|------|-------------|----------|------|
| **Daily** | Notes quotidiennes | `journal-daily.md` | `#note/journal` `#frequency/quotidien` |
| **Weekly** | Bilan hebdomadaire | `journal-weekly.md` | `#note/journal` `#frequency/hebdomadaire` |
| **Monthly** | Bilan mensuel | `journal-monthly.md` | `#note/journal` `#frequency/mensuel` |
| **Reflection** | Réflexion approfondie | Libre | `#note/journal` `#note/reflection` |
| **Meeting** | Compte-rendu de réunion | `meeting.md` | `#note/meeting` |

---

## 🎯 Comment utiliser le Journal

### ➕ Créer une note quotidienne
1. **Via le plugin Daily Notes** (recommandé) :
   - Utiliser le raccourci Obsidian (par défaut : `Ctrl/Cmd + N` puis sélectionner Daily Note)
   - Ou via la commande : `Daily Notes: Create today's note`

2. **Manuellement** :
   - Créer un fichier : `YYYY-MM-DD.md`
   - Utiliser le template **journal-daily.md**

### 📊 Structurer une note quotidienne

*Voir le template complet : [[templates/journal-daily|Template Journal Daily]]*

```markdown
---
 date: 2024-11-16
tags:
  - note/journal
  - frequency/quotidien
---

# 2024-11-16

## 🎯 3 Priorités du jour
- [ ] Tache 1
- [ ] Tache 2
- [ ] Tache 3

## 📝 Notes
- Note 1
- Note 2

## 💡 Idées
- Idée 1
- Idée 2

## 📚 Apprentissages
- Apprentissage 1
- Apprentissage 2

## ✅ Bilan
- Ce qui a bien marché
- Ce qui peut être amélioré
```

---

## 🔍 Recherche dans le Journal

*Utilise Dataview pour des requêtes avancées :*

**Toutes les notes de novembre 2024 :**
```dataview
LIST
FROM "journal/2024/2024-11"
SORT file.name DESC
```

**Notes avec le tag #apprentissage :**
```dataview
LIST
FROM "journal"
WHERE contains(tags, "#apprentissage")
SORT file.name DESC
```

**Bilan du mois :**
```dataview
TABLE
  length(file.tasks) as "Taches",
  length(file.links) as "Liens"
FROM "journal/2024/2024-11"
WHERE file.name != "README"
```

---

## 📅 Bilans périodiques

### 📆 Weekly Review (Tous les lundis)

**Template suggéré :**
```markdown
---
tags:
  - note/journal
  - frequency/hebdomadaire
---

# Weekly Review - [YYYY-MM-DD]

## ✅ Bilan de la semaine
- [ ] Projets terminés
- [ ] Projets en cours
- [ ] Projets bloqués

## 🎯 Priorités pour la semaine prochaine
- Priorité 1
- Priorité 2
- Priorité 3

## 💡 Réflexions
- Ce qui a bien fonctionné
- Ce qui peut être amélioré
```

### 📆 Monthly Review (Premier jour du mois)

**Template suggéré :**
```markdown
---
tags:
  - note/journal
  - frequency/mensuel
---

# Monthly Review - [YYYY-MM]

## 📊 Bilan du mois
- Projets terminés
- Objectifs atteints
- Apprentissages majeurs

## 🎯 Objectifs pour le mois prochain
- Objectif 1
- Objectif 2
- Objectif 3

## 📈 Métriques
- Temps passé par projet
- Productivité
- Satisfaction
```

---

## 💡 Bonnes pratiques

> [!tip] Conseils
> - **Écrire tous les jours** (même 2-3 lignes)
> - **Relire régulièrement** : Hebdomadaire, mensuel, annuel
> - **Lier aux autres notes** : Projets, Areas, Resources
> - **Utiliser des templates** pour gagner du temps
> - **Garder ça simple** : Pas besoin de notes parfaites

> [!warning] À éviter
> - Sauter trop de jours consécutifs
> - Écrire des romans (garder ça concis)
> - Négliger les liens vers d'autres notes

---

## 📚 Ressources liées

- [[00-inbox/README|Inbox]] - Pour capturer rapidement
- [[01-projects/README|Projets]] - Projets mentionnés dans le journal
- [[02-areas/README|Areas]] - Domaines suivis
- [[templates/journal-daily|Template Journal Daily]]

---

*Dernière mise à jour : <% tp.date.now("YYYY-MM-DD") %>*
