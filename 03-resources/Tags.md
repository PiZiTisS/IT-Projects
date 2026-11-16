---
cssclasses:
  - tags-index
status: active
year: 2024
tags:
  - meta
  - index
---

# 🏷️ Système de Tags

> [!objectif] Objectif
> Définir une **taxonomie cohérente** de tags pour organiser et retrouver facilement les notes dans le vault. Utiliser des tags spécifiques et hiérarchiques.

---

## 📌 **Règles générales**

> [!tip] Bonnes pratiques
> - **Utiliser des tags hiérarchiques** : `domaine/sous-domaine` (ex: `area/developpement`)
> - **Éviter les tags trop génériques** : Préférer `#resource/livre/tech` à `#tech`
> - **Limiter le nombre de tags par note** : 3-5 maximum
> - **Utiliser des singuliers** : `#livre` et non `#livres`
> - **Éviter les espaces** : Utiliser des tirets `#note-litterature`

> [!warning] À éviter
> - Tags redondants avec le nom du dossier
> - Tags avec des majuscules ou caractères spéciaux
> - Tags trop nombreux ou trop spécifiques

---

## 🎯 **Catégories principales**

### 📍 **PARA** (Structure principale)

| Tag | Description | Exemple |
|-----|-------------|---------|
| `#area/nom` | Domaines de responsabilité permanente | `#area/developpement`, `#area/sante` |
| `#project/nom` | Projets actifs | `#project/site-web`, `#project/app-mobile` |
| `#resource/type` | Resources et connaissances | `#resource/livre`, `#resource/cours` |
| `#archive/annee` | Archives | `#archive/2023`, `#archive/2024` |

---

### 📅 **Statuts**

| Tag | Description | Utilisation |
|-----|-------------|-------------|
| `#status/en-cours` | Actif, en développement | Projets, taches |
| `#status/en-attente` | Planifié, pas encore démarré | Projets, idées |
| `#status/termine` | Achevé | Projets, taches |
| `#status/abandonne` | Annulé | Projets |
| `#status/en-pause` | Temporairement suspendu | Projets |
| `#status/a-lire` | Resource à consulter | Livres, articles |
| `#status/en-cours-lecture` | En train de lire | Livres |
| `#status/lu` | Déjà lu | Livres, articles |
| `#status/a-revoir` | À relire/revoir | Resources |

---

### ⭐ **Types de notes**

| Tag | Description | Exemple |
|-----|-------------|---------|
| `#note/fleeting` | Note temporaire, idée rapide | `2024-11-16-idee.md` |
| `#note/litterature` | Note de lecture | `Livre-Titre.md` |
| `#note/permanente` | Note durable, concept | `Concept-Nom.md` |
| `#note/projet` | Note liée à un projet | `Projet-Specifications.md` |
| `#note/area` | Note liée à une area | `Area-Objectifs.md` |
| `#note/journal` | Note de journal | `2024-11-16.md` |
| `#note/meeting` | Compte-rendu de réunion | `2024-11-16-Reunion.md` |

---

### 🎯 **Domaines** (à adapter)

| Tag | Description | Exemples |
|-----|-------------|----------|
| `#domain/tech` | Technologie | `#domain/developpement`, `#domain/devops` |
| `#domain/pro` | Professionnel | `#domain/carriere`, `#domain/management` |
| `#domain/perso` | Personnel | `#domain/sante`, `#domain/finances` |
| `#domain/apprentissage` | Apprentissage | `#domain/formation`, `#domain/lecture` |
| `#domain/creativite` | Créativité | `#domain/ecriture`, `#domain/design` |

---

### 📚 **Types de Resources**

| Tag | Description | Exemple |
|-----|-------------|---------|
| `#resource/livre` | Livres | `#resource/livre/tech` |
| `#resource/cours` | Cours et formations | `#resource/cours/udemy` |
| `#resource/article` | Articles de blog | `#resource/article/medium` |
| `#resource/video` | Vidéos, conférences | `#resource/video/youtube` |
| `#resource/podcast` | Podcasts | `#resource/podcast/nom` |
| `#resource/outil` | Outils, logiciels | `#resource/outil/obsidian` |
| `#resource/contact` | Contacts | `#resource/contact/mentor` |
| `#resource/document` | Documents PDF, etc. | `#resource/document/guide` |

---

### ⚡ **Priorités & Urgence**

| Tag | Description | Utilisation |
|-----|-------------|-------------|
| `#priority/haute` | Priorité élevée | Taches, projets |
| `#priority/moyenne` | Priorité moyenne | Taches |
| `#priority/faible` | Priorité faible | Taches |
| `#urgent` | Urgent | Taches, projets |
| `#important` | Important (mais pas urgent) | Projets, areas |

---

### 👥 **Personnes & Rôles**

| Tag | Description | Exemple |
|-----|-------------|---------|
| `#person/nom` | Personne spécifique | `#person/jean-dupont` |
| `#role/mentor` | Rôle de mentor | `#role/mentor` |
| `#role/collegue` | Collègue de travail | `#role/collegue` |
| `#role/ami` | Ami | `#role/ami` |
| `#role/famille` | Membre de la famille | `#role/famille` |

---

### 📊 **Fréquence** (pour les actions récurrentes)

| Tag | Description | Exemple |
|-----|-------------|---------|
| `#frequency/quotidien` | Tous les jours | Routines |
| `#frequency/hebdomadaire` | Toutes les semaines | Reviews |
| `#frequency/mensuel` | Tous les mois | Bilans |
| `#frequency/trimestriel` | Tous les trimestres | Évaluations |
| `#frequency/annuel` | Une fois par an | Objectifs annuels |

---

## 🔍 **Exemples concrets**

### Note de projet
```markdown
---
tags:
  - project/site-ecommerce
  - area/developpement
  - status/en-cours
  - priority/haute
  - domain/tech
---
```

### Note de livre
```markdown
---
tags:
  - resource/livre
  - resource/livre/tech
  - domain/developpement
  - status/a-lire
---
```

### Note de journal
```markdown
---
tags:
  - note/journal
  - frequency/quotidien
---
```

### Note de réunion
```markdown
---
tags:
  - note/meeting
  - project/site-ecommerce
  - person/jean-dupont
  - role/collegue
---
```

---

## 🛠️ **Outils pour gérer les tags**

### **Recherche par tag dans Obsidian**
- Utiliser le panneau **Tags** (Ctrl/Cmd + T)
- Utiliser la recherche : `tag:#area/developpement`

### **Dataview - Requêtes par tag**

**Toutes les notes avec un tag spécifique :**
```dataview
LIST
WHERE contains(tags, "#area/developpement")
```

**Compter les notes par tag :**
```dataview
TABLE length(tags) as "Nombre de tags", tags
FROM ""
GROUP BY tags
SORT length(tags) DESC
```

**Trouver les notes avec un statut spécifique :**
```dataview
LIST
WHERE contains(tags, "#status/en-cours")
```

---

## 📝 **Maintenance du système**

> [!todo] Review Mensuelle des Tags
> - [ ] Vérifier les tags utilisés récemment
> - [ ] Supprimer les tags inutilisés
> - [ ] Fusionner les tags redondants
> - [ ] Mettre à jour cette documentation

---

*Dernière mise à jour : <% tp.date.now("YYYY-MM-DD") %>*
