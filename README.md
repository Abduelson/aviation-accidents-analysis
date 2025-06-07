# Aircraft Accidents & Incidents (1962–2023) – Analyse Exploratoire de Données

## Aperçu

Ce projet de science des données vise à analyser les accidents et incidents d'aéronefs survenus entre 1962 et 2023. En combinant exploration, visualisations et interprétations, l'objectif est de fournir des **informations exploitables pour une entreprise souhaitant acquérir un aéronef avec un minimum de risque**.

---

## Compréhension des Affaires

**Objectif principal :**  
Aider une entreprise à identifier les types d’aéronefs les plus sûrs en analysant les données historiques d’accidents et d’incidents.

### Questions clés des parties prenantes :

- Quels types d’aéronefs sont les plus impliqués dans des accidents ?
- Existe-t-il une catégorie ou un type d’aéronef plus sûr ?
- Quelles sont les caractéristiques des incidents ayant causé le plus de blessés ?
- Y a-t-il un lien entre le type de moteur ou la catégorie d’aéronef et la gravité des accidents ?

---

## Compréhension et Analyse des Données

### Source des données

- Base de données officielle issue de [NTSB](https://www.ntsb.gov) ou autre dépôt public de données sur la sécurité aérienne.
- Période couverte : **1962 à 2023**
- Taille : plus de 89 000 occurrences

### Description des données

Les colonnes principales utilisées dans l’analyse comprennent :

- `Event.Type` : Accident ou Incident
- `Aircraft.Category` : Catégorie de l’aéronef (Airplane, Helicopter, Glider, etc.)
- `Engine.Type` : Type de moteur (Piston, Electric, Turbo, etc.)
- `Total.Fatal.Injuries` : Nombre total de morts
- `Total.Minor.Injuries`, `Total.Serious.Injuries`, `Total.Uninjured`
- `Make`, `Model` : Fabricant et nom de l’aéronef
- `Location`, `Year`

---

## Visualisations

### 1. Moyenne des blessures par catégorie d’aéronef

Bar chart montrant la moyenne des blessures par `Aircraft.Category` :

- Les catégories "WSFT" et "Unknown" ont les plus hauts taux de blessures en moyenne.

### 2. Type de moteur par accident (Pie Chart)

Répartition des accidents selon `Engine.Type`.  
Certaines catégories apparaissent avec une fréquence équivalente.

### 3. Top 10 des aéronefs les plus impliqués

Un **bar chart** montrant les modèles d’aéronef les plus fréquemment impliqués dans des accidents.

---

## Conclusion

### Résumé des conclusions :

1. **Les aéronefs de type Glider et Powered-Lift** sont ceux ayant la **plus faible moyenne de blessures graves**.
2. **Les catégories Airplane et Helicopter** sont les plus fréquentes dans les accidents, mais pas nécessairement les plus graves.
3. **Le type de moteur** n’a pas montré de corrélation significative avec la gravité des blessures, selon les données disponibles.

---

> Ce projet fournit une base solide pour des analyses plus poussées et peut aider les décideurs à identifier les aéronefs les moins risqués en fonction des tendances historiques.
