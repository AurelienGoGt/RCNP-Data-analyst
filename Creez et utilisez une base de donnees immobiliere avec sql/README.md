# 🏗️ Projet : Base de Données Immobilière — DATAImmo

> 💡 *Parce qu’avant de prédire le prix d’un bien, encore faut-il savoir dans quelle table il se cache…*

---

## 🧭 Contexte du projet

L’objectif de ce projet est de **concevoir et structurer une base de données immobilière** permettant de centraliser et d’analyser les transactions foncières en France.  
L’enjeu est de créer un **système de données fiable, normalisé et interopérable** pour soutenir les besoins analytiques et décisionnels d’un réseau d’agences immobilières.

Cette base servira de fondation à des projets analytiques futurs, tels que la **modélisation des prix de vente**, la **segmentation géographique** ou la **prévision des tendances du marché**.

---

## 🎯 Objectifs principaux

- Concevoir un **modèle relationnel complet** (3NF) pour structurer les données immobilières, régionales et démographiques.  
- Créer et peupler une base de données opérationnelle avec **SQLite / MySQL / PostgreSQL**.  
- Réaliser un **dictionnaire de données** décrivant les variables clés.  
- Effectuer des **requêtes SQL analytiques** afin d’obtenir des indicateurs de marché pertinents (prix moyen, volume de ventes, distribution géographique, etc.).  
- Mettre à jour et documenter un **catalogue de données** pour garantir la traçabilité et la gouvernance.

---

## 🧩 Structure du projet

| Étape | Description | Livrable principal |
|--------|--------------|--------------------|
| **1. Conception** | Étude des sources et création du schéma relationnel normalisé | Schéma 3NF (diagramme E/A) |
| **2. Documentation** | Création du dictionnaire des données | Dictionnaire (CSV / Excel) |
| **3. Implémentation** | Création et remplissage des tables dans le SGBD | Tables : `Bien`, `Vente`, `Commune`, `Région` |
| **4. Analyse SQL** | Rédaction et exécution de requêtes analytiques | Rapport PDF des requêtes et résultats |

---

## 🗃️ Schéma relationnel (vue d’ensemble)

Le modèle relationnel repose sur quatre entités principales :

| Table | Description | Clé primaire | Lien |
|--------|--------------|---------------|------|
| **Région** | Données géographiques régionales (nom, code, etc.) | `id_region` | reliée à `Commune` |
| **Commune** | Informations sur les communes françaises | `id_commune` | reliée à `Région` et `Bien` |
| **Bien** | Description des propriétés (surface, type, nombre de pièces, etc.) | `id_bien` | reliée à `Vente` |
| **Vente** | Informations sur les transactions (prix, date, acheteur, etc.) | `id_vente` | reliée à `Bien` et `Commune` |

Le schéma suit la **troisième forme normale (3NF)** pour garantir la non-redondance et la cohérence des données.

---

## 🧮 Exemples de requêtes réalisées

- Moyenne des prix de vente par région  
- Répartition des transactions par type de bien  
- Évolution mensuelle du nombre de ventes  
- Prix moyen au m² par département  
- Top 10 des communes les plus actives sur la période étudiée  

---

## 🧰 Stack technique

| Domaine | Outils & Technologies |
|----------|----------------------|
| Langage | SQL |
| Base de données | SQLite / MySQL / PostgreSQL |
| Documentation | Excel / Markdown / Diagramme E/A |
| Analyse complémentaire | Python (Pandas, Matplotlib) |
| Visualisation | Power BI (en option) |

---

## 🧾 Livrables du projet

| N° | Type | Nom du livrable |
|----|------|-----------------|
| 1 | Documentation | Dic
