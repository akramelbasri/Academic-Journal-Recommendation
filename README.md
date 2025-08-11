# Academic Journal Recommendation System

## 📚 Description

Un système intelligent de recommandation de journaux académiques développé avec Streamlit. Cette application utilise l'apprentissage automatique pour analyser le contenu de vos articles et vous proposer les journaux les plus pertinents pour votre publication.

## ✨ Fonctionnalités

- **Analyse de contenu intelligente** : Traitement automatique du titre, résumé et mots-clés de votre article
- **Recommandations par score SJR** : Suggestions basées sur l'impact et la qualité des journaux
- **Recommandations par similarité** : Propositions basées sur la similarité du contenu avec des articles existants
- **Interface utilisateur intuitive** : Interface web moderne et responsive avec Streamlit
- **Prétraitement avancé du texte** : Nettoyage, suppression des stopwords et lemmatisation
- **Clustering automatique** : Classification des articles par domaines thématiques

## 🛠️ Technologies utilisées

- **Frontend** : Streamlit
- **Machine Learning** : Scikit-learn (K-means clustering, TF-IDF, Nearest Neighbors)
- **Traitement du langage naturel** : NLTK
- **Manipulation de données** : Pandas, NumPy
- **Interface de données** : Streamlit-AgGrid
- **Sauvegarde des modèles** : Joblib

## 🚀 Installation et utilisation

### Prérequis
```bash
pip install streamlit pandas numpy scikit-learn nltk streamlit-aggrid joblib
```

### Lancement de l'application
```bash
streamlit run app.py
```

### Utilisation
1. Ouvrez votre navigateur à l'adresse indiquée (généralement http://localhost:8501)
2. Entrez le titre de votre article
3. Ajoutez le résumé (abstract)
4. Saisissez les mots-clés séparés par des virgules
5. Cliquez sur "Trouver des journaux recommandés"
6. Consultez les recommandations dans les deux onglets disponibles

## 📊 Structure du projet

```
Academic-Journal-Recommendation/
├── app.py                 # Application principale Streamlit
├── data/
│   └── df_clustering.csv  # Données des journaux avec clustering
├── Models/
│   └── kmeans_model.joblib # Modèle de clustering entraîné
├── Tokenizers/
│   └── tfidf_vectorizer.joblib # Vectoriseur TF-IDF entraîné
└── README.md
```

## 🔍 Algorithmes utilisés

### Clustering K-means
- Classification automatique des articles par domaines thématiques
- Permet de filtrer les recommandations par cluster

### TF-IDF Vectorisation
- Transformation du texte en vecteurs numériques
- Prise en compte de la fréquence des termes et de leur importance

### Nearest Neighbors
- Calcul de similarité cosinus entre articles
- Recommandations basées sur la proximité sémantique

## 📈 Métriques de recommandation

- **Score SJR (SCImago Journal Rank)** : Indicateur de qualité et d'impact des journaux
- **Score de similarité** : Pourcentage de similarité avec les articles existants
- **Rang de recommandation** : Classement des journaux par pertinence

## 🎯 Cas d'usage

- **Chercheurs** : Trouver le journal le plus approprié pour publier leurs travaux
- **Étudiants** : Identifier les revues pertinentes pour leurs recherches
- **Institutions académiques** : Optimiser les stratégies de publication

## 🤝 Contribution

Les contributions sont les bienvenues ! N'hésitez pas à :
- Signaler des bugs
- Proposer de nouvelles fonctionnalités
- Améliorer la documentation
- Optimiser les algorithmes

## 📝 Licence

Ce projet est sous licence MIT. Voir le fichier LICENSE pour plus de détails.

## 👨‍💻 Auteur

Développé avec ❤️ pour la communauté académique.

---

*Ce système aide les chercheurs à faire les meilleurs choix de publication en combinant analyse de contenu et métriques de qualité des journaux.*