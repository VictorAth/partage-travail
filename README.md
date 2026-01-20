# Analyse des facteurs influençant le prix des maisons

**Auteur :** Victor Attoh  
**Projet :** Mini-projet encadré - Séance 14  
**Dataset :** Ames Housing (Kaggle)

## Présentation du projet

Ce projet consiste en une analyse exploratoire et statistique des prix de l'immobilier à Ames, Iowa. L'objectif est d'identifier les caractéristiques physiques et temporelles qui impactent le plus fortement le `SalePrice` (prix de vente).

## Structure du dossier

Conformément aux directives, le dépôt est organisé comme suit :

- `/data/` : Contient le dataset original (`train.csv`) ainsi que les exports intermédiaires générés lors du nettoyage.
- `rapport.Rmd` : Code source R Markdown incluant l'importation, le nettoyage, les visualisations et le modèle de régression.
- `rapport.html` : Rapport final exporté (format web) avec un sommaire interactif et un design épuré.

## 🛠️ Méthodologie appliquée

1. **Importation & Audit** : Sélection des variables clés (Surface, Qualité, Années).
2. **Nettoyage rigoureux** : Suppression des doublons et gestion des valeurs manquantes pour garantir la fiabilité statistique.
3. **Ingénierie de variables (Feature Engineering)** :
   - Création de `Surface_Totale` (Somme de la surface habitable et du sous-sol).
   - Création de `Age_Maison` (Calcul de l'ancienneté au moment de la vente).
4. **Visualisation** : Analyse des corrélations via des nuages de points et des boîtes à moustaches (boxplots).
5. **Modélisation** : Mise en place d'une régression linéaire multiple pour quantifier l'influence des variables.

## Comment lire le rapport ?

Pour consulter les résultats détaillés :

1. Téléchargez le dossier.
2. Ouvrez le fichier `rapport.html` dans n'importe quel navigateur web.
3. Utilisez le sommaire flottant à gauche pour naviguer entre les étapes.

## Principales conclusions

- La **Surface Totale** est le facteur prédictif le plus puissant du prix de vente.
- L'**Âge de la maison** au moment de la vente présente une corrélation négative significative, confirmant la dépréciation immobilière liée au temps.
- La **Qualité Globale** agit comme un multiplicateur de valeur majeur.
