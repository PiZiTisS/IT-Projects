---
cssclasses:
  - templates-index
status: active
year: 2024
tags:
  - index
  - templates
  - meta
---

# 📄 Templates - Index

> [!objectif] Objectif
> Centraliser tous les **modèles de notes** pour standardiser la création de nouvelles notes et gagner du temps.

---

## 📋 Liste des templates disponibles

| Template | Description | Utilisation |
|----------|-------------|-------------|
| [[projet|projet.md]] | Projet avec objectifs et étapes | Projets actifs |
| [[area|area.md]] | Domaine de responsabilité | Areas |
| [[resource|resource.md]] | Resource/knowledge | Resources |
| [[journal-daily|journal-daily.md]] | Note quotidienne | Journal |
| [[journal-weekly|journal-weekly.md]] | Bilan hebdomadaire | Journal |
| [[journal-monthly|journal-monthly.md]] | Bilan mensuel | Journal |
| [[literature-note|literature-note.md]] | Note de lecture | Resources/Livres |
| [[permanent-note|permanent-note.md]] | Note permanente | Knowledge |
| [[meeting|meeting.md]] | Compte-rendu de réunion | Projets/Areas |
| [[person|person.md]] | Contact/Personne | Resources/Contacts |

---

## 🎯 Comment utiliser les templates

### **Méthode 1 : Plugin Templater (recommandé)**
1. Installer le plugin **Templater** via Community Plugins
2. Configurer le dossier de templates : `templates/`
3. Créer une nouvelle note avec `Ctrl/Cmd + P` → `Templater: Create new note from template`
4. Choisir le template souhaité

### **Méthode 2 : Plugin Core Templates**
1. Aller dans `Settings → Core plugins → Templates`
2. Configurer le dossier de templates : `templates/`
3. Créer une nouvelle note et sélectionner le template

### **Méthode 3 : Copier manuellement**
1. Ouvrir le template dans `templates/`
2. Copier le contenu
3. Créer une nouvelle note et coller

---

## 📝 Structure d'un template

> [!tip] Bonnes pratiques
> - **Utiliser des placeholders** : ` <% tp.file.title %>` pour Templater
> - **Ajouter des métadonnées YAML** : Pour le filtrage et l'organisation
> - **Inclure des callouts** : `> [!objectif]`, `> [!etapes]` pour la clarté
> - **Documenter le template** : Ajouter une section "Comment utiliser"

---

## 🛠️ Variables Templater utiles

| Variable | Description | Exemple |
|----------|-------------|---------|
| `tp.file.title` | Nom du fichier (sans extension) | `<% tp.file.title %>` |
| `tp.file.rename()` | Renommer le fichier | `<% tp.file.rename("NouveauNom") %>` |
| `tp.date.now()` | Date actuelle | `<% tp.date.now("YYYY-MM-DD") %>` |
| `tp.date.weekday()` | Jour de la semaine | `<% tp.date.weekday("fr") %>` |
| `tp.user.get()` | Variable utilisateur | `<% tp.user.get("nom") %>` |
| `tp.system.suggester()` | Menu de sélection | `<% tp.system.suggester(["Option1", "Option2"]) %>` |

---

## 📁 Structure recommandée pour les templates

```
templates/
├── README.md              # Ce fichier
├── projet.md              # Template pour les projets
├── area.md                # Template pour les areas
├── resource.md            # Template pour les resources
├── journal/
│   ├── daily.md           # Template journal quotidien
│   ├── weekly.md          # Template journal hebdo
│   └── monthly.md         # Template journal mensuel
└── notes/
    ├── literature.md      # Template note de lecture
    ├── permanent.md        # Template note permanente
    ├── meeting.md          # Template réunion
    └── person.md           # Template contact
```

---

## 💡 Conseils pour créer de bons templates

1. **Garder ça simple** : Un template ne doit pas être trop complexe
2. **Inclure des exemples** : Montrer comment remplir chaque section
3. **Utiliser des valeurs par défaut** : Préremplir avec des valeurs courantes
4. **Documenter** : Ajouter des commentaires sur l'utilisation
5. **Tester** : Créer une note avec le template pour vérifier qu'il fonctionne

---

## 📚 Ressources liées

- [Documentation Templater](https://silentvoid13.github.io/Templater/)
- [Obsidian Templates Docs](https://help.obsidian.md/Plugins/Templates)
- [[01-projects/README|Projets]] - Utilisation des templates projet
- [[02-areas/README|Areas]] - Utilisation des templates area

---

*Dernière mise à jour : <% tp.date.now("YYYY-MM-DD") %>*
