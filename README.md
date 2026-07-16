# Construction et analyse d'une surface de volatilité implicite
Projet personnel de finance quantitative.

## Présentation

Ce projet a pour objectif de construire et d'analyser une surface de volatilité implicite à partir de données d'options de marché.

Les données sont récupérées à l'aide de l'API **Yahoo Finance** sur les options de l'ADR américain de **TotalEnergies (Ticker : TTE)**. Les volatilités implicites sont ensuite calculées par inversion numérique du modèle de **Black-Scholes**, puis comparées aux volatilités implicites fournies par Yahoo Finance.

Le projet permet également d'étudier les **smiles**, les **skews de volatilité**, la surface de volatilité implicite ainsi que les principales sensibilités du modèle de Black-Scholes.

---

## Objectifs

- Télécharger les chaînes d'options disponibles sur Yahoo Finance.
- Construire un jeu de données exploitable à partir des options de marché.
- Calculer la moneyness et la maturité des contrats.
- Implémenter le modèle de Black-Scholes pour les calls européens.
- Calculer les volatilités implicites par inversion numérique.
- Comparer les résultats obtenus aux volatilités implicites de Yahoo Finance.
- Étudier les smiles et les skews de volatilité.
- Construire une surface de volatilité implicite.
- Analyser l'influence des paramètres du modèle ainsi que les principaux Greeks (Delta, Gamma et Vega).

---

## Méthodologie

Le projet suit les étapes suivantes :

1. Téléchargement des chaînes d'options.
2. Nettoyage des données de marché.
3. Construction du DataFrame des options.
4. Calcul de la moneyness et du temps restant jusqu'à maturité.
5. Implémentation du modèle de Black-Scholes.
6. Calcul des volatilités implicites par inversion numérique.
7. Évaluation de la qualité de la calibration (MAE, RMSE, erreur moyenne et erreur maximale).
8. Analyse des smiles et des skews de volatilité.
9. Construction de la surface de volatilité implicite par interpolation.
10. Étude des sensibilités du modèle (Delta, Gamma et Vega).

---

## Résultats

Le notebook contient notamment :

- la récupération et le nettoyage des données d'options ;
- le calcul des volatilités implicites ;
- la comparaison avec les volatilités implicites de Yahoo Finance ;
- une analyse des erreurs de calibration ;
- des représentations des smiles et des skews de volatilité ;
- une visualisation tridimensionnelle de la surface de volatilité implicite ;
- une étude de l'influence des paramètres du modèle de Black-Scholes ;
- une analyse des principaux Greeks.

---

## Bibliothèques utilisées

- Python
- NumPy
- pandas
- SciPy
- Matplotlib
- Plotly
- yfinance

---

## Structure du dépôt

```
.
├── Surface_de_volatilité_implicite.ipynb
├── README.md
└── requirements.txt
```

---

## Pistes d'amélioration

Plusieurs extensions peuvent être envisagées :

- intégrer les dividendes dans le modèle ;
- comparer plusieurs sous-jacents ;
- étudier différentes dates d'observation ;
- implémenter un modèle à volatilité stochastique (Heston) ;
- développer une application interactive avec Streamlit.

---

## Auteur

**Yvanna Marianne Nseke**

Master 2 Ingénierie Financière et Modèles Aléatoires  
Sorbonne Université

N'hésitez pas à me contacter pour toute remarque ou suggestion d'amélioration.