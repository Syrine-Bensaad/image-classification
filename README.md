# Reconnaissance faciale avec SVM
Ce projet utilise une Machine à Vecteurs de Support (SVM) pour effectuer la reconnaissance faciale sur le dataset Labeled Faces in the Wild (LFW). Le dataset est pré-téléchargé et stocké localement.
##  Installation
Pour commencer, clonez le dépôt et installez les bibliothèques requises :
```sh
git clone https://github.com/Syrine-Bensaad/image-classification
cd image-classification
pip install -r requirements.txt
```
## 📂 Dataset
Le dataset Labeled Faces in the Wild (LFW) est utilisé pour ce projet. Assurez-vous que le dataset est stocké dans le répertoire spécifié :

```sh
./lfw-funneled
```
## 🚀 Utilisation
Pour exécuter le modèle de reconnaissance faciale, utilisez la commande suivante :

```sh

python face_recognition.py
```
## 🌐 Déploiement avec Streamlit
Le fichier deploy.py est conçu pour le déploiement avec Streamlit. Pour déployer le modèle et exécuter l'application Streamlit, utilisez la commande suivante :

```sh

streamlit run deploy.py
```
## 📊 Entraînement du Modèle
Le modèle est entraîné en utilisant un SVM avec des poids de classe équilibrés. Le processus d'entraînement implique les étapes suivantes :

- **Chargement du dataset LFW** : Les données faciales sont chargées depuis le répertoire spécifié.
- **Division des données** : Les données sont divisées en ensembles d'entraînement et de test.
- **Entraînement du modèle SVM** : Le modèle est entraîné sur les données d'entraînement.
- **Évaluation du modèle** : Le modèle est évalué sur les données de test pour mesurer sa performance.
## 📈 Résultats
Le rapport de classification pour le modèle est le suivant :

```sh
                 précision    rappel  f1-score   support

     Colin Powell       0.89      0.88      0.88        64
  Donald Rumsfeld       0.89      0.78      0.83        32
    George W Bush       0.87      0.91      0.89       127
Gerhard Schroeder       0.89      0.86      0.88        29
       Tony Blair       0.88      0.85      0.86        33

         exactitude                           0.88       285
        moyenne macro       0.88      0.86      0.87       285
     moyenne pondérée       0.88      0.88      0.88       285
```
## 🖼️ Visualisations
Le script inclut des visualisations de certaines des faces du dataset. Elles peuvent être vues en exécutant le script et en inspectant les graphiques générés.

## 📋 Exigences
Les bibliothèques Python requises sont listées dans requirements.txt et incluent :

- **scikit-learn**
- **matplotlib**
- **streamlit**








