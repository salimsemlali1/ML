
#  Projet Deep Learning : Classification d'images avec CNN sur CIFAR-10

Ce projet utilise un **réseau de neurones convolutif (CNN)** pour classer automatiquement des images du dataset **CIFAR-10** dans 10 catégories. Il comprend toutes les étapes : chargement, prétraitement, entraînement, sauvegarde, visualisation des performances, et prédiction.

---

##  Dataset : CIFAR-10

- **Taille** : 60 000 images couleur 32x32 pixels
- **Répartition** :
  - Entraînement : 50 000 images
  - Test : 10 000 images
- **Catégories** :
  - Avion, Auto, Oiseau, Chat, Cerf, Chien, Grenouille, Cheval, Bateau, Camion

---

##  Technologies utilisées

- Python 3.10
- TensorFlow 2.x
- NumPy
- Matplotlib
- Jupyter Notebook

---

##  Étapes d'installation et d'exécution

### Étape 1 : Installer les dépendances

```bash
pip install --upgrade pip
pip install tensorflow matplotlib numpy
```

---

### Étape 2 : Lancer le Notebook Jupyter

```bash
jupyter notebook
```

Puis ouvrir le fichier :  
`Nom_Du_Projet.ipynb`

---

##  Étapes du projet dans le notebook

1.  Chargement des données CIFAR-10
2.  Prétraitement : normalisation + one-hot encoding
3.  Construction du modèle CNN
4.  Compilation du modèle
5.  Entraînement sur les données
6.  Sauvegarde du modèle au format `.keras`
7.  Évaluation sur les données de test
8.  Affichage des courbes (précision et perte)
9.  Prédiction sur une image test aléatoire

---

##  Architecture du modèle CNN

```text
Entrée : (32, 32, 3)
↓ Conv2D(32 filtres, 3x3) + ReLU
↓ MaxPooling2D(2x2)
↓ Conv2D(64 filtres, 3x3) + ReLU
↓ MaxPooling2D(2x2)
↓ Flatten
↓ Dense(128) + ReLU
↓ Dropout(0.5)
↓ Dense(10) + Softmax
```

---

##  Résultats attendus

- Précision du modèle : ~70–80% après 10 époques
- Graphiques générés :
  - Précision entraînement vs validation
  - Perte entraînement vs validation
- Affichage d'une image test avec la prédiction du modèle

---



##  Auteur

- **Nom** : Semlali Salim
- **Contact** : salim.semlali@um5r.ac.ma
- **GitHub** : 
