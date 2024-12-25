# Projet-Python-

# 🌞 Évaluation et Prévision des Énergies Renouvelables Variables

## 🌍 Introduction

Dans un contexte de transition énergétique, les **énergies renouvelables variables** comme le photovoltaïque jouent un rôle central dans la production électrique en France métropolitaine. Cependant, leur nature intermittente et dépendante des conditions climatiques rend leur gestion complexe, nécessitant des prévisions précises pour anticiper les variations de puissance et maintenir la stabilité du réseau électrique.

## 🎯 Objectif du Projet

Ce projet vise à **prédire les facteurs de capacité** des installations photovoltaïques à partir des **données climatiques locales** afin d’évaluer avec précision la **production horaire d’énergie solaire**. 

### 🔍 Pourquoi passer par les **facteurs de capacité** ?

#### Une mesure plus universelle et robuste
Le facteur de capacité exprime la fraction de la production réelle par rapport à la production théorique maximale. Cela en fait une métrique universelle, permettant de :  
- Comparer les performances entre régions aux conditions climatiques variables.  
- Analyser les tendances temporelles sans être influencé par des extensions de parcs ou des variations de capacité installée. 

#### Une mesure indépendante de la taille des parcs photovoltaïques
La production brute d’énergie solaire varie directement en fonction de la **capacité installée** des parcs photovoltaïques. Par conséquent, comparer les productions de différentes régions ou prévoir leur évolution est biaisé par les différences de taille des installations. 

Les **facteurs de capacité** permettent de contourner cette limitation en exprimant la performance des parcs photovoltaïques sous une forme **normalisée**. Ils reflètent l’efficacité des installations solaires en fonction des **conditions climatiques locales** , indépendamment de leur capacité nominale. 

#### Optimisation du réseau électrique
Une prévision précise des facteurs de capacité est essentielle pour :  
- Anticiper les variations de production horaire ou journalière.  
- Mieux intégrer les énergies renouvelables dans le réseau électrique.  
- Réduire les coûts associés au stockage ou à la surcapacité en ajustant les ressources en temps réel.

## 🌞 Relevé des Données
En s’appuyant sur les **observations historiques des facteurs de capacité** et les **données climatiques**, ce projet propose de prédire les performances des parcs photovoltaïques par région de la France métropolitaine. Cette approche permet de mieux évaluer l’impact des énergies renouvelables dans le **mix énergétique** et de contribuer à la stabilité du réseau électrique face à la montée en puissance des énergies intermittentes.


## 🛠 Architecture du Projet

1. **Récupération et Traitement des Données**
   - Collecte de données météorologiques
   - Collecte des données de facteurs de capacité 
   - Nettoyage et mise en forme des données pour assurer leur fiabilité.
     
2. **Analyse Descriptive et Représentation Graphique**
   - Exploration des relations entre variables climatiques et facteurs de capacité.

3. **Modélisation**
   - Développement de modèles prédictifs pour anticiper les variations.
   - Validation à l’aide d’indicateurs statistiques.


## Données

1. **Données climatiques (NASA MERRA-2)**  
   - Issues du site officiel : [https://gmao.gsfc.nasa.gov/reanalysis/MERRA-2/](https://gmao.gsfc.nasa.gov/reanalysis/MERRA-2/)  
   - L’accès nécessite des identifiants, donc pour simplifier, les fichiers de données déjà téléchargés sont placés dans le dossier `data`.

2. **Données de facteurs de capacité**  
   - Récupérées automatiquement par le notebook via l’API d’OpenDataSoft  
   - Chaque région française est couverte.

## Packages nécessaires

Le notebook `main.ipynb` importe et installe (si besoin) l’ensemble des dépendances Python requises, notamment :

- `pandas`, `numpy`  
- `scikit-learn`  
- `matplotlib`, `seaborn`  
- … etc.

Il suffit de lancer `main.ipynb` pour exécuter toutes les analyses et visualisations.


