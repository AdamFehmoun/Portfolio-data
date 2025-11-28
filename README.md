# 📊 Global Data Science Salaries Analysis (2024)

> Analyse exploratoire et modélisation ML sur un dataset de +93,000 offres d'emploi dans la Tech.

## 🎯 Objectif
Comprendre les dynamiques de rémunération dans le marché de la Data (Data Scientist, ML Engineer, Data Analyst) pour identifier les leviers de carrière les plus rentables :
* Impact de l'expérience (Junior vs Senior).
* Impact de la localisation (USA vs France).
* Prédiction de salaire via Machine Learning.

## 🛠️ Stack Technique
* **Langage :** Python 3.13
* **Analyse :** Pandas, NumPy
* **Visualisation :** Seaborn, Matplotlib
* **Machine Learning :** Scikit-learn (Régression Linéaire)

## 💡 Résultats Clés (Insights)

### 1. Le "Gap" Américain 🇺🇸
Le marché US est sans commune mesure avec le reste du monde.
* Salaire moyen Senior (US) : **~177,000 $**
* Salaire moyen Senior (France) : **~100,000 €** (dans ce dataset de profils internationaux)
* **Conclusion :** Une carrière aux USA ou en remote pour une boîte US rapporte x2 à x3 plus.

### 2. La prime à l'expérience en France 🇫🇷
L'évolution salariale est très forte entre le niveau Junior et Senior.
* **Junior (EN) :** ~52k€
* **Senior (SE) :** ~100k€
* *Note : Les données pour les Directeurs (Executives) en France ne sont pas représentatives (échantillon trop faible de n=2).*

### 3. Prédiction IA 🤖
J'ai entraîné un modèle de Régression Linéaire simple.
* Pour un profil avec **7 ans d'expérience**, le modèle prédit un salaire théorique mondial d'environ **198208.73 $**.

## 🛑 Analyse Critique : Le "Double Marché" Français
En croisant les données mondiales (Kaggle) avec les grilles de recrutement locales (Silkhom), j'ai mis en évidence une **anomalie majeure** sur les profils Seniors (SE).

* **Salaire Senior Standard (Vert) :** ~70 000 € (Marché local).
* **Salaire Senior Kaggle (Rouge) :** ~140 000 € (Marché biaisé "Big Tech").

**Conclusion :** Il existe un "marché caché" en France. Les salaires doublent si l'on cible les entreprises internationales ou le secteur Big Tech, faussant les moyennes mondiales. Mon objectif de carrière est de cibler ce segment "Rouge".

## 💸 Étude Comparative : Pouvoir d'Achat Réel (France vs USA)
J'ai modélisé l'évolution de l'épargne mensuelle (Cash Flow) en prenant en compte :
* Les impôts réels (42% France vs ~32-39% USA).
* Le coût de la vie local (Loyer, Santé, Assurances).

**Résultat de la simulation :**
Même avec un coût de la vie 2x plus élevé à San Francisco, le différentiel de salaire est tel que **l'épargne résiduelle aux USA est 3x supérieure** à celle d'un profil équivalent à Paris.
* **Junior :** L'écart est faible (Paris est compétitif grâce au faible coût de vie).
* **Senior :** L'écart devient massif (L'expatriation devient un levier d'accumulation de capital majeur).

## 📂 Structure du projet
* `salaries.csv` : Le dataset brut (Source : Kaggle).
* `Projet_Salaires.ipynb` : Le notebook contenant tout le code d'analyse et les graphiques.

---
**Auteur :** Adam Fehmoun - Étudiant Ingénieur DSIA @ ESIEE Paris