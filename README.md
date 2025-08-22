# Waste Classifier

## Descroption
Ce projet a pour but de développer un système de classification automatique des déchets basé sur la vision par ordinateur. Utilisant des techniques de Deep Learning, le modèle est entraîné pour identifier la nature d'un déchet (plastique, verre, métal, carton, papier, etc.) à partir d'une image. L'objectif final est de fournir un module intelligent, prêt à être intégré dans un robot de tri automatisé pour améliorer l'efficacité et la rapidité du recyclage.

## Table des matières

- [Installation](#installation)
- [Utilisation](#utilisation)
- [Configuration](#configuration)
- [Tests](#tests)
- [Contribuer](#contribuer)
- [Licence](#licence)
- [Auteurs](#auteurs)

## Installation

Pour mettre en place le projet localement, suivez ces étapes :

```bash
# 1. Clonez le dépôt depuis GitHub
git clone https://github.com/manfoya/waste-classifier.git

# 2. Accédez au répertoire du projet
cd waste-classifier

# 3. (Optionnel mais recommandé) Créez et activez un environnement virtuel
python -m venv venv
source venv/bin/activate  # Sur Windows: venv\Scripts\activate

# 4. Installez les dépendances requises
pip install -r requirements.txt
```
Assurez-vous d'avoir téléchargé le jeu de données et de l'avoir placé dans le répertoire `/data` comme spécifié dans la configuration.

## Utilisation

Le projet est structuré autour de deux scripts principaux : un pour l'entraînement du modèle et un pour la prédiction sur de nouvelles images.

```bash
# Pour entraîner un nouveau modèle
# Vous pouvez spécifier l'architecture, le nombre d'époques, etc.
python train.py --model EfficientNetB0 --epochs 30

# Pour lancer une prédiction sur une seule image
python predict.py --image_path /chemin/vers/votre/image.jpg

# Pour lancer l'API de classification (si applicable)
python app.py
```

## Configuration

La configuration principale du projet se trouve dans le fichier `config.yaml`. Ce fichier vous permet de gérer les paramètres sans modifier le code source.



## Tests

Pour garantir la fiabilité du code, des tests unitaires ont été mis en place. Pour les exécuter, utilisez la commande suivante à la racine du projet :

```bash
pytest
```
Cela lancera l'ensemble des tests situés dans le répertoire `/tests`.

## Contribuer

Les contributions sont les bienvenues. Pour contribuer, veuillez suivre ces étapes :

1.  **Fork** le projet sur GitHub.
2.  Créez une nouvelle branche pour votre fonctionnalité (`git checkout -b feature/nom-de-la-feature`).
3.  Faites vos modifications et commitez-les (`git commit -m 'Ajout de ma feature'`).
4.  Poussez vos changements vers votre fork (`git push origin feature/nom-de-la-feature`).
5.  Ouvrez une **Pull Request**.

Veuillez vous assurer que votre code respecte les standards de style et que tous les tests passent avant de soumettre votre contribution.

## Licence

Ce projet est sous licence MIT. Pour plus de détails, veuillez consulter le fichier [LICENSE](LICENSE) inclus dans ce dépôt.

## Auteurs

*   **manfoya** - *Développement initial et maintenance*