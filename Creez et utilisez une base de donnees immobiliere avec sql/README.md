<h1 align="center"> 🏗️ Projet : Base de Données Immobilière — DATAImmo : </h1> 

> 💡 *Parce qu’avant de prédire le prix d’un bien, encore faut-il savoir dans quelle table il se cache…*

---

<h2 align="center"> 🧭 Contexte du projet : </h2> 

L’objectif de ce projet est de **concevoir et structurer une base de données immobilière** permettant de centraliser et d’analyser les transactions foncières en France.  
L’enjeu est de créer un **système de données fiable, normalisé et interopérable** pour soutenir les besoins analytiques et décisionnels d’un réseau d’agences immobilières.


---

<h2 align="center"> 🎯 Objectifs principaux : </h2> 

- Charger des données dans une base de données
- Créer des tables dans une base de données
- Créer le schéma d'une base de données
- Effectuer des requêtes SQL pour répondre à une problématique métier
- Mettre à jour un catalogue de données

---

<h2 align="center"> 🧩 Structure du projet : </h2> 

| Étape | Description | Livrable principal |
|--------|--------------|--------------------|
| **1. Conception** | Étude des sources et création du schéma relationnel normalisé | Schéma 3NF (diagramme E/A) |
| **1. Documentation** | Création du dictionnaire des données | Dictionnaire (CSV / Excel) |
| **3. Implémentation** | Création et remplissage des tables dans le SGBD | Tables : `Bien`, `Vente`, `Commune`, `Région` |
| **4. Analyse SQL** | Rédaction et exécution de requêtes analytiques | Rapport PDF des requêtes et résultats |

---

<h2 align="center"> 🗃️ Schéma relationnel : </h2> 

Le modèle relationnel repose sur quatre entités principales :

| Table | Description | Clé primaire |
|--------|--------------|---------------|
| **Région** | Données géographiques régionales (nom, code, etc.) | `id_region` | 
| **Commune** | Informations sur les communes françaises | `id_commune` | 
| **Bien** | Description des propriétés (surface, type, nombre de pièces, etc.) | `id_bien` |
| **Vente** | Informations sur les transactions (prix, date, acheteur, etc.) | `id_vente` |

Le schéma suit la **troisième forme normale (3NF)** pour garantir la non-redondance et la cohérence des données.

---

<h2 align="center"> 🧮 Exemples de requêtes réalisées : </h2> 

- Moyenne des prix de vente par région  
- Répartition des transactions par type de bien  
- Évolution mensuelle du nombre de ventes  
- Prix moyen au m² par département  
- Top 10 des communes les plus actives sur la période étudiée  

---

<h2 align="center"> 🧰 Stack technique : </h2> 

| Domaine | Outils & Technologies |
|----------|----------------------|
| Langage | SQL |
| Base de données | MySQL / PostgreSQL |
| Documentation | Excel / Markdown / Diagramme E/A / Pa Architect / Mindmap|

---

<h2 align="center"> 🧾 Livrables du projet : </h2> 

| N° | Type | Nom du livrable |
|----|------|-----------------|
| 1 | .txt file | Pour les differentes requetes SQL
| 2 | .pa architect | Pour la creation des tables SQL
| 3 | .umd file | Pour les relations des differentes tables

