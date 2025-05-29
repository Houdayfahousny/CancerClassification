# 🧬 CancerClassification

Ce projet vise à développer un modèle de deep learning capable de classer les images de lésions cutanées à partir du dataset **HAM10000**. Il s'agit d'un projet de classification d'images pour la détection précoce de cancers de la peau.

## 📂 Dataset

- **Nom** : [Skin Cancer MNIST: HAM10000](https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000)
- **Description** : Le dataset contient 10 015 images dermatoscopiques de 7 types de lésions cutanées, y compris des mélanomes.
- **Format** : JPEG 600x450 pixels + fichier CSV de métadonnées

## 🛠️ Technologies

- Python (Google Colab)
- TensorFlow / Keras
- NumPy, Pandas, Matplotlib
- Scikit-learn

## 🧠 Modèle

Le modèle de classification est un CNN simple construit avec Keras :

- **Prétraitement** : redimensionnement, normalisation
- **Architecture** : 
  - Conv2D + MaxPooling
  - Dropout
  - Flatten + Dense
- **Optimiseur** : Adam
- **Fonction de perte** : Categorical Crossentropy
- **Métrique** : Accuracy

## 📊 Résultats

Performances du modèle :

- **Validation :**
  - Accuracy : **74.56%**
  - Loss : **0.75**

- **Test :**
  - Accuracy : **72.19%**
  - Loss : **0.77**

> 🔍 Des pistes d'amélioration incluent : l'utilisation de modèles pré-entraînés, l'augmentation des données, et la gestion du déséquilibre de classes.

## 🧪 Instructions pour exécuter

1. Clone ce repo :
   ```bash
   git clone https://github.com/Houdayfahousny/CancerClassification.git
