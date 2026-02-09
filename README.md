# Exploring Pokémon Data With Unsupervised Learning
### *Author: Chiara Pizzetti*

This project explores and analyzes Pokémon data using various **unsupervised learning techniques** to uncover hidden patterns, natural groupings and semantic similarities within the Pokémon universe.

This analysis aims to:
- Measure similarity between Pokémon based on base statistics.
- Discover natural clusters of Pokémon and moves.
- Apply Natural Language Processing (NLP) to move descriptions to find functional groupings.
- Identify "anomalous" or unique Pokémon that defy standard categorizations.

## **Datasets** 
The analysis is performed on three datasets retrieved from the PokéAPI:
- `pokemon_complete.csv`: Contains data for 1025 Pokémon, including physical traits (height, weight), types, abilities, and base battle statistics (HP, Attack, Defense, etc.).
- `moves_complete.csv`: Includes details for 797 moves, featuring both numerical battle properties (Power, Accuracy, PP) and textual descriptions (Effect Text).
- `learnset_complete.csv`: A bridge dataset mapping which Pokémon can learn which moves.

## **Key Features & Methodology**
- **Data Preprocessing**: Handling missing values for secondary types, abilities (filled as "None"), and status moves (filling null Power/Accuracy with 0).
- **Exploratory Data Analysis**: Analysis of type distribution imbalance (e.g., Water-type dominance vs. Flying-type rarity) and move category proportions.
- **Clustering**: Grouping Pokémon based on stat distributions.
- **Similarity Analysis**: Linking statistical profiles with move-set versatility.
- **NLP for Moves**: Using textual descriptions to identify moves with similar effects regardless of their elemental type.

## **Libraries**
- `pandas` for data manipulation.
- `matplotlib` and `seaborn` for data visualization.
- `scikit-learn` for unsupervised learning algorithms.
- `nltk` or `scikit-learn` (Tfidf/CountVectorizer) for textual analysis.

## **How to Use**
1. Clone the repository
2. Ensure the three CSV files are in the project root.
3. Run the Jupyter Notebook `Exploring_Pokemon_Data.ipynb`.




