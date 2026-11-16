---
cssclasses:
  - attachments-index
status: active
year: 2024
tags:
  - index
  - attachments
---

# 📎 Attachments - Index

> [!objectif] Objectif
> Stocker et organiser les **fichiers joints** (images, PDF, documents, captures d'écran, etc.) qui accompagnent les notes du vault.

---

## 📁 Structure recommandée

```
attachments/
├── images/
│   ├── screenshots/
│   │   └── 2024-11-16-caption.png
│   ├── diagrams/
│   │   └── architecture-diagram.png
│   └── icons/
│       └── icon-name.png
├── documents/
│   ├── pdf/
│   │   └── document.pdf
│   ├── excel/
│   │   └── data.xlsx
│   └── word/
│       └── report.docx
├── media/
│   ├── audio/
│   │   └── recording.mp3
│   └── video/
│       └── tutorial.mp4
└── archives/
    └── old-files.zip
```

---

## 🎯 Comment nommer les fichiers

> [!etapes] Convention de nommage
> - [ ] Utiliser le format : `YYYY-MM-DD-Description.[ext]`
> - [ ] Éviter les espaces et caractères spéciaux
> - [ ] Utiliser des tirets pour séparer les mots
> - [ ] Garder les noms **courts mais descriptifs**

**Exemples :**
- ✅ `2024-11-16-diagramme-architecture.png`
- ✅ `2024-11-15-cv-pierre-dupont.pdf`
- ❌ `mon super diagramme final v2.png`
- ❌ `Capture d'écran 2024-11-16 143022.png`

---

## 🔗 Lier les attachments aux notes

### Méthode 1 : Lien relatif (recommandé)
```markdown
![Description](attachments/images/2024-11-16-diagramme.png)
```

### Méthode 2 : Lien absolu (si nécessaire)
```markdown
![Description](/c/Users/naeld/Projets_info/attachments/images/2024-11-16-diagramme.png)
```

### Méthode 3 : Embed PDF
```markdown
![[2024-11-15-document.pdf]]
```

---

## 📋 Gestion des attachments

### ➕ Ajouter un fichier
1. **Glisser-déposer** dans le dossier `attachments/`
2. **Renommer** selon la convention
3. **Lier** depuis la note correspondante
4. **Ajouter une description** dans la note

### 🗑️ Nettoyer les attachments

> [!todo] Maintenance régulière
> - [ ] **Tous les mois** : Vérifier les fichiers orphelins (non liés)
> - [ ] **Tous les 6 mois** : Supprimer les doublons
> - [ ] **Tous les ans** : Archiver les anciens fichiers

---

## 🛠️ Outils pour gérer les attachments

### **Plugin Obsidian : Image Toolkit**
- Redimensionner les images
- Ajouter des filigranes
- Optimiser les images

### **Plugin Obsidian : Attachment Management**
- Renommer automatiquement les attachments
- Détecter les fichiers orphelins
- Organiser automatiquement

### **Script pour trouver les fichiers orphelins**
```dataview
LIST
FROM "attachments"
WHERE !link
```
*(Note : Cette requête nécessite des métadonnées appropriées)*

---

## 📊 Statistiques

*Nombre de fichiers par type :*
```dataview
TABLE
  length(file.links) as "Fichiers liés"
FROM "attachments"
GROUP BY file.extension
SORT file.extension ASC
```

---

## 💡 Bonnes pratiques

> [!tip] Conseils
> - **Organiser par année/mois** : `attachments/2024/11/` pour les fichiers de novembre 2024
> - **Utiliser des sous-dossiers** par type (images, documents, etc.)
> - **Compresser les anciens fichiers** régulièrement
> - **Éviter les fichiers trop volumineux** (>10Mo)
> - **Préférer les formats ouverts** (PDF, PNG, SVG)

> [!warning] À éviter
> - Stocker des fichiers sensibles (mots de passe, données privées)
> - Utiliser des noms de fichiers trop génériques (`image1.png`)
> - Ne pas lier les fichiers aux notes
> - Stocker des vidéos/photos haute résolution (préférer des liens externes)

---

## 📚 Ressources liées

- [[00-inbox/README|Inbox]] - Pour capturer des fichiers temporaires
- [[01-projects/README|Projets]] - Projets utilisant des attachments
- [[03-resources/README|Resources]] - Documents de référence

---

*Dernière mise à jour : <% tp.date.now("YYYY-MM-DD") %>*
