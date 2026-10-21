# 🧠 Behavior Analysis — Machine Learning
### Analyse de comportements et de préférences par apprentissage supervisé et non supervisé

![Status](https://img.shields.io/badge/Statut-Termin%C3%A9-green)
![Orange](https://img.shields.io/badge/Platform-Orange%20Data%20Mining-orange)
![Machine Learning](https://img.shields.io/badge/Domain-Machine%20Learning-purple)
![NLP](https://img.shields.io/badge/Text%20Mining-NLP-blue)

## Présentation du projet

**Behavior Analysis — Machine Learning** est un projet universitaire réalisé dans le cadre de la formation MIASHS (*Mathématiques et Informatique Appliquées aux Sciences Humaines et Sociales*) à l'Université Paul-Valéry Montpellier 3.

Il consiste à explorer deux approches complémentaires du **Machine Learning** à l'aide du logiciel **Orange Data Mining** : l'apprentissage non supervisé et l'apprentissage supervisé.

Le projet repose sur l'analyse de deux jeux de données distincts : des avis textuels de produits cosmétiques et des données relatives aux habitudes de travail pendant la pandémie de COVID-19.

L'objectif est d'identifier des structures cachées dans les données, de comprendre les comportements des individus et de construire des modèles capables de prédire certaines préférences.

## Problématique

> Comment les méthodes d'apprentissage supervisé et non supervisé permettent-elles d'identifier, de comprendre et de prédire des comportements à partir de données textuelles et socio-professionnelles ?

L'étude s'articule autour de deux axes :

- **Apprentissage non supervisé :** identifier des groupes d'avis cosmétiques présentant des caractéristiques similaires, sans catégories prédéfinies.
- **Apprentissage supervisé :** prédire les préférences entre télétravail et travail au bureau à partir de variables liées aux habitudes et aux conditions de vie.

## Jeux de données

Le projet exploite deux datasets correspondant à des problématiques différentes.

| Dataset | Type de données | Objectif |
|---|---|---|
| Ulta Skincare Reviews | Avis clients textuels sur des produits cosmétiques | Identifier des groupes d'avis similaires |
| WFH / WFO Dataset | Données socio-professionnelles et habitudes de vie | Prédire la préférence entre télétravail et bureau |

**Dataset 1 — Avis cosmétiques**

Les commentaires clients sont analysés à l'aide de techniques de traitement automatique du langage naturel (NLP), afin d'identifier les thèmes et les caractéristiques qui rapprochent les différents avis.

**Dataset 2 — Télétravail et habitudes de vie**

Les données permettent d'étudier les relations entre les préférences professionnelles et plusieurs facteurs, notamment la productivité perçue, le sommeil, les économies réalisées et l'équilibre entre vie professionnelle et vie personnelle.

## Objectifs

- Découvrir et mettre en œuvre les principales étapes d'un pipeline de Machine Learning.
- Préparer et transformer des données textuelles et structurées.
- Appliquer des techniques de traitement automatique du langage naturel (NLP).
- Utiliser la représentation Bag of Words et la pondération TF-IDF.
- Identifier des groupes d'observations par clustering hiérarchique.
- Interpréter les clusters à l'aide de visualisations.
- Entraîner et comparer plusieurs modèles de classification supervisée.
- Évaluer les performances prédictives des modèles.
- Identifier les variables les plus associées aux préférences étudiées.

## Technologies utilisées

**Orange Data Mining** — Construction de workflows visuels pour le prétraitement, l'apprentissage automatique et l'évaluation des modèles.

**Text Mining / NLP** — Nettoyage, tokenisation et représentation numérique des avis textuels.

**Bag of Words / TF-IDF** — Transformation des documents en caractéristiques exploitables par les algorithmes.

**Clustering hiérarchique** — Regroupement des avis selon leurs similarités.

**Random Forest** — Modèle de classification supervisée utilisé pour prédire les préférences professionnelles.

**Data Visualization** — Exploration des données, visualisation des clusters et interprétation des résultats.

**Git & GitHub** — Versionnement et partage des ressources du projet.

## Méthodologie

Le projet suit cinq grandes étapes :

**01 — Collecte et exploration des données**

Sélection de deux jeux de données, identification des variables pertinentes et exploration de leurs caractéristiques.

**02 — Prétraitement**

Nettoyage des données textuelles, suppression des mots non informatifs (*stopwords*) et transformation des avis en représentations numériques à l'aide de Bag of Words et TF-IDF.

Préparation des variables structurées pour leur utilisation dans les modèles de classification.

**03 — Apprentissage non supervisé**

Application d'un clustering hiérarchique aux avis cosmétiques afin de faire émerger des groupes présentant des caractéristiques communes.

Utilisation de visualisations, notamment des nuages de mots, pour interpréter les clusters obtenus.

**04 — Apprentissage supervisé**

Entraînement et comparaison de plusieurs algorithmes de classification pour prédire les préférences entre télétravail et travail au bureau.

Évaluation des performances et identification du modèle le plus adapté aux données étudiées.

**05 — Interprétation des résultats**

Analyse des groupes d'avis identifiés, comparaison des performances prédictives et étude des variables les plus importantes dans les prédictions.

## Résultats principaux

Les analyses ont permis de mettre en évidence plusieurs observations.

| Analyse | Résultat |
|---|---|
| Classification supervisée | Random Forest obtient la meilleure performance rapportée, avec une précision d'environ 90 % |
| Clustering des avis | Identification de deux profils principaux de commentaires |
| Analyse des préférences professionnelles | Mise en évidence de plusieurs variables associées aux préférences de travail |

**Analyse non supervisée**

Le clustering distingue notamment deux grandes catégories d'avis :

- **Sensorialité et douceur :** commentaires mettant davantage en avant l'expérience sensorielle et le confort d'utilisation.
- **Efficacité et résultats :** commentaires privilégiant les effets observés et les performances des produits.

**Analyse supervisée**

Le modèle Random Forest présente les meilleures performances parmi les modèles comparés, avec une précision rapportée d'environ **90 %**.

Les variables les plus associées aux préférences de travail comprennent la productivité perçue, la qualité du sommeil, les économies réalisées et l'équilibre entre vie professionnelle et vie personnelle.

## Organisation du dépôt

Le dépôt comprend les fichiers suivants :

- `orange1_KB.ows` : workflow Orange consacré à l'apprentissage non supervisé et au clustering des avis cosmétiques.
- `orange2_KB.ows` : workflow Orange consacré à l'apprentissage supervisé et à la classification.
- `stopwords1_KB.txt.txt` : liste personnalisée de mots à exclure lors du prétraitement textuel.
- `rapport_KB.pdf` : rapport universitaire présentant la méthodologie et les résultats.
- `Projet_KB.zip` : archive contenant des ressources du projet.

Les fichiers `.ows` peuvent être ouverts directement avec **Orange Data Mining**, sous réserve de disposer des extensions nécessaires.

## Limites méthodologiques

Les analyses présentent plusieurs limites :

- Les avis cosmétiques constituent un échantillon de commentaires et ne représentent pas nécessairement l'ensemble des consommateurs.
- Les résultats du clustering dépendent des choix de prétraitement, de représentation textuelle et de méthode de regroupement.
- Les préférences de télétravail peuvent évoluer selon le contexte professionnel et la période étudiée.
- Les performances des modèles de classification dépendent de la composition des données et de la méthode d'évaluation.
- Les associations entre variables ne permettent pas d'établir des relations causales.
- Les modèles entraînés sur ces jeux de données ne garantissent pas des performances équivalentes sur de nouvelles populations.

Ces limites doivent être prises en compte lors de l'interprétation et de la généralisation des résultats.

---

**Behavior Analysis — Turning data into behavioral insights.**
