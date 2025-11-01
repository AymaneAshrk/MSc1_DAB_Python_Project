# 📊 Projet M1 - Analyse Économique et Environnementale Globale

> **M1** — MSc Data Analytics for Business (KEDGE BS), 2024–2025

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![M1](https://img.shields.io/badge/Level-M1-blue)](https://kedge.edu/)
[![KEDGE](https://img.shields.io/badge/Program-MSc%20DAB%20(KEDGE)-green)](https://kedge.edu/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)

## 📋 Table des matières

- [Aperçu](#-aperçu)
- [Fonctionnalités](#-fonctionnalités)
- [Structure du projet](#-structure-du-projet)
- [Installation](#-installation)
- [Utilisation](#-utilisation)
- [Analyses réalisées](#-analyses-réalisées)
- [Données](#-données)
- [Technologies](#️-technologies)
- [Résultats](#-résultats)

## 🎯 Aperçu

Ce projet d'analyse de données examine les relations complexes entre facteurs économiques, environnementaux et géopolitiques à l'échelle mondiale. L'analyse porte sur les corrélations entre PIB, émissions de CO2, dépenses militaires, population et données boursières, révélant des insights cruciaux pour les décideurs politiques et économiques.

**Contexte académique :** Projet réalisé dans le cadre du M1 Data Analytics for Business à KEDGE Business School (2024–2025).

### Questions de recherche analysées

- **Relations PIB-Environnement** : Impact des émissions de CO2 sur la croissance économique
- **Géopolitique économique** : Corrélation entre dépenses militaires et PIB national
- **Dynamiques démographiques** : Influence de la population sur les indicateurs économiques
- **Performance des marchés** : Analyse des données boursières et leur contexte macroéconomique

## ✨ Fonctionnalités

- 🔄 Pipeline ETL multi-sources (CSV, JSON, données fusionnées)
- 📊 4 visualisations statistiques principales avec exports PNG
- 🌍 Analyses géospatiales avec cartes choroplèthes
- 📈 Matrices de corrélation et analyses de régression
- 🎯 Classements et comparaisons internationales
- 📋 Traitement et nettoyage de données complexes
- 💾 Exports structurés en formats multiples (CSV, JSON, PNG)

## 📁 Structure du projet

```
analyse-economique-environnementale-globale/
├── VERSION_FINALE.ipynb          # Notebook principal d'analyse
├── DATASETS/
│   ├── CSV/                      # Données sources au format CSV
│   │   ├── co2-emissions-and-gdp.csv
│   │   ├── military.csv
│   │   ├── national-gdp-wb.csv
│   │   ├── population.csv
│   │   └── stock.csv
│   ├── JSON/                     # Données au format JSON
│   └── MERGED/                   # Datasets fusionnés et traités
├── OUTPUTS/                      # Visualisations générées
│   ├── 1-Matrice-corrélation.png
│   ├── 2-Corrélation PIB_CO2.png
│   ├── 3-Classement 10pays_pollueurs.png
│   └── 4-Carte Militaire_PIB.png
      
```

## 🚀 Installation

### Prérequis

- Python 3.8 ou supérieur
- Jupyter Notebook / JupyterLab
- Minimum 4GB RAM (pour le traitement des datasets volumineux)

### Étapes d'installation

1. **Cloner le repository**
```bash
git clone https://github.com/AymaneAshrk/MSc1_DAB_Python_Project.git
cd MSc1_DAB_Python_Project
```


## 💻 Utilisation

### Démarrage rapide

1. Vérifier la présence des datasets dans `DATASETS/CSV/`
2. Lancer Jupyter : `jupyter notebook VERSION_FINALE.ipynb`
3. Exécuter toutes les cellules : `Cell → Run All`
4. Consulter les visualisations dans `OUTPUTS/`

### Structure du notebook

Le notebook est organisé en sections logiques :

- **Configuration** : Imports et paramètres globaux
- **Chargement des données** : Lecture et validation des datasets
- **Nettoyage et préparation** : Traitement des valeurs manquantes, standardisation
- **Analyses exploratoires** : Statistiques descriptives et premiers insights
- **Visualisations** : Création des 4 graphiques principaux
- **Conclusions** : Synthèse des résultats et recommandations

## 📊 Analyses réalisées

### 1. Matrice de corrélation globale

**Fichier** : `1-Matrice-corrélation.png`

- Corrélations entre toutes les variables économiques et environnementales
- Heatmap avec coefficients de Pearson
- Identification des relations significatives

### 2. Corrélation PIB-CO2

**Fichier** : `2-Corrélation PIB_CO2.png`

- Analyse de régression linéaire PIB vs émissions CO2
- Scatter plot avec ligne de tendance
- Coefficient de détermination R²

### 3. Top 10 des pays pollueurs

**Fichier** : `3-Classement 10pays_pollueurs.png`

- Classement des émissions de CO2 par pays
- Barplot horizontal avec données actualisées
- Analyse comparative internationale

### 4. Carte géopolitique Militaire-PIB

**Fichier** : `4-Carte Militaire_PIB.png`

- Visualisation géospatiale des dépenses militaires en % du PIB
- Carte choroplèthe mondiale
- Analyse des tendances géopolitiques

## 📁 Données

### Sources principales

| Dataset | Description | Taille | Variables principales |
| :-- | :-- | :-- | :-- |
| **co2-emissions-and-gdp.csv** | Émissions CO2 et PIB par pays/année | ~994KB | Pays, Année, CO2, PIB |
| **military.csv** | Dépenses militaires mondiales | ~474KB | Pays, Année, Dépenses militaires |
| **national-gdp-wb.csv** | PIB national (World Bank) | ~209KB | Pays, Année, PIB |
| **population.csv** | Données démographiques | ~460KB | Pays, Année, Population |
| **stock.csv** | Données boursières | ~86KB | Ticker, Prix, Volume |

### Période d'analyse

- **Temporalité** : 1990-2023 (selon disponibilité des données)
- **Couverture géographique** : Mondiale (195+ pays)
- **Fréquence** : Annuelle pour la plupart des indicateurs

## 🛠️ Technologies

### Librairies principales

- **pandas** : Manipulation et analyse de données
- **numpy** : Calculs numériques et matrices
- **matplotlib/seaborn** : Visualisations statistiques
- **plotly** : Graphiques interactifs et cartes
- **scipy** : Analyses statistiques avancées
- **geopandas** : Données géospatiales (cartes)

### Techniques analytiques

- **Analyse de corrélation** : Pearson, Spearman
- **Régression linéaire** : OLS, validation statistique
- **Analyse exploratoire** : Statistiques descriptives
- **Visualisation géospatiale** : Cartes choroplèthes
- **Data cleaning** : Gestion des valeurs manquantes, outliers

## 📈 Résultats

### Principales découvertes

1. **Corrélation PIB-CO2** : Relation positive forte (r > 0.7) entre développement économique et émissions
2. **Dépenses militaires** : Concentration géographique avec disparités importantes (0.5% à 15% du PIB)
3. **Top pollueurs** : Domination des grandes puissances économiques (Chine, USA, Inde)
4. **Dynamiques temporelles** : Évolution contrastée selon les régions et niveaux de développement

### Implications analytiques

- **Pour les décideurs** : Trade-off évident entre croissance et environnement
- **Géopolitique** : Corrélation entre instabilité régionale et dépenses militaires
- **Développement durable** : Nécessité de découpler croissance et émissions
- **Méthodologie** : Importance de la qualité des données pour analyses multicritères

---

**Auteur** : Aymane Ashrk  
**Formation** : M1 Data Analytics for Business - KEDGE Business School  
**Année académique** : 2024-2025  
**Portfolio** : [GitHub](https://github.com/AymaneAshrk)

---

*Ce projet démontre l'application de techniques avancées d'analyse de données à des problématiques économiques et environnementales contemporaines, avec une approche méthodologique rigoureuse et des visualisations professionnelles.*
