# 🏗️ Scraper Tri - Automatisation de la Collecte des Centres de Tri BTP

[![Python](https://img.shields.io/badge/Python-3.11%2B-blue.svg)](https://www.python.org/)
[![Selenium](https://img.shields.io/badge/Selenium-4.15%2B-green.svg)](https://selenium.dev/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Production%20Ready-brightgreen.svg)]()
[![Documentation](https://img.shields.io/badge/Docs-Available-blue.svg)](https://krikounoureddine.github.io/Scraper-Tri/Rapport_Du_Projet.pdf)

> 🧠 Application desktop intelligente pour l’automatisation de la recherche, la collecte et la gestion des données des centres de tri du BTP référencés sur le site de la **Fédération Française du Bâtiment (FFB)**.

---

## 📋 Table des Matières

- [🎯 Aperçu](#-aperçu)
- [🚀 Fonctionnalités](#-fonctionnalités)
- [🧩 Technologies Utilisées](#-technologies-utilisées)
- [🏗️ Architecture](#-architecture)
- [📊 Résultats](#-résultats)
- [🛠️ Installation](#️-installation)
- [💻 Utilisation](#-utilisation)
- [🎬 Démonstration](#-démonstration)
- [👥 Auteurs et Encadrement](#-auteurs-et-encadrement)
- [🙏 Remerciements](#-remerciements)
- [📄 Licence](#-licence)
- [📫 Contact](#-contact)

---

## 🎯 Aperçu

**Scraper Tri** est une application développée dans le cadre d’un stage de Master 2 à **l’Université Paris VIII**, en collaboration avec l’entreprise **SISCO**.  
Elle automatise la recherche et la collecte des centres de tri de déchets de chantier sur le site officiel de la [FFB](https://www.dechets-chantier.ffbatiment.fr/).

### 📈 Problématique Résolue

- [Difficultés rencontrées et solutions apportées](https://krikounoureddine.github.io/Scraper-Tri/presentation/Diagramme_difficultes_solutions.html)
- [Arbre de décision des types de déchets](https://krikounoureddine.github.io/Scraper-Tri/presentation/Types_Dechets.html)

---

## 🚀 Fonctionnalités

🔗 [Diagramme de flux complet de l'application](https://krikounoureddine.github.io/Scraper-Tri/presentation/Diagramme_de_flux_complet.html)

### 🔍 Recherche Intelligente
- **3 modes de recherche** : Simple, Multi-catégories, Avancée  
- **Géolocalisation** : Recherche par ville, code postal, département  
- **Filtres avancés** : 37 types de déchets répartis en 11 catégories  
- **Validation automatique** des adresses et formats  

### 🤖 Scraping Automatisé
- **Navigation Selenium** : Simulation réaliste du navigateur  
- **Gestion ASP.NET** : Traitement dynamique des formulaires complexes  
- **Parsing XML** : Extraction fine depuis les flux FFB  
- **Gestion d’erreurs** : 28 cas d’erreurs identifiés et traités  

### 💾 Gestion des Données
- **Base SQLite** : 2 bases (`centre_tri.db`, `centres_tri_complet.db`)  
- **Dédoublonnage** : Suppression automatique des doublons  
- **Historique** : Archivage et mise à jour horodatée des recherches  
- **Modèle relationnel normalisé**

### 📤 Export Multi-Formats
```python
exports = {
    "word": "Rapports formatés (.docx)",
    "excel": "Données tabulées (.xlsx)",
    "csv": "Interopérabilité (.csv)",
    "json": "API/Web (.json)",
    "carte": "Visualisation géographique (.html)"
}
