# Cr-ation-de-Cartes-de-Disparit-avec-OpenCV-et-SIFT


Bienvenue dans ce projet où nous explorons la création de cartes de disparité en utilisant la librairie OpenCV et les points d’intérêt SIFT. Ce projet est un travail pratique qui couvre plusieurs aspects de la vision par ordinateur, de la détection des points d’intérêt à la génération de cartes de disparité.

Table des Matières

	•	Aperçu
	•	Prérequis
	•	Installation
	•	Utilisation
	•	Étapes du Projet
	•	Calcul des Points SIFT
	•	Mise en Correspondance des Points d’Intérêt
	•	Filtrage des Correspondances avec RANSAC
	•	Création de la Carte de Disparité
	•	Résultats et Analyse
	•	Contributions
	•	Auteur
	•	Licence

Aperçu

Dans ce projet, nous allons créer des cartes de disparité en utilisant des images stéréoscopiques. Les étapes incluent le calcul des points SIFT sur deux images, la mise en correspondance de ces points, l’application de RANSAC pour filtrer les mauvaises correspondances, et finalement la génération de la carte de disparité.

![ảnh](https://github.com/user-attachments/assets/9165abcd-9cbd-4ef6-a56c-6c91be491586)


Prérequis

Avant de commencer, assurez-vous d’avoir les éléments suivants installés sur votre machine :

	•	Python 3.x
	•	Jupyter Notebook
	•	Bibliothèques Python : opencv-python, numpy, matplotlib

Installation

	1.	Clonez ce dépôt pour obtenir tous les fichiers nécessaires :
 git clone https://github.com/votre-utilisateur/projet-cartes-disparité.git
cd projet-cartes-disparité

2.	Installez les dépendances pour garantir que tous les scripts s’exécutent correctement :
3.	pip install opencv-python numpy matplotlib


	2.	Suivez les étapes détaillées dans le notebook pour découvrir les différentes méthodes et modèles que nous avons développés.

Étapes du Projet

Calcul des Points SIFT

La première étape consiste à calculer les points SIFT sur les deux images (gauche et droite) :

	•	Détection des points d’intérêt : Utilisation de SIFT pour détecter les points d’intérêt et calculer les descripteurs.

Mise en Correspondance des Points d’Intérêt

Nous mettons ensuite en correspondance les points d’intérêt détectés sur les deux images :

	•	Utilisation de BFMatcher : Mise en correspondance des descripteurs SIFT des deux images.
	•	Application du ratio test de Lowe : Filtrage des correspondances pour retenir les meilleures.
 ![ảnh](https://github.com/user-attachments/assets/577d8720-17b3-41d8-82b8-1e7a0e5f6a6f)
 


Filtrage des Correspondances avec RANSAC

Pour améliorer la précision, nous appliquons RANSAC pour filtrer les mauvaises correspondances :

	•	Application de RANSAC : Filtrage des correspondances pour obtenir un ensemble de points de correspondance fiable.
![ảnh](https://github.com/user-attachments/assets/41f793a7-e129-4bd2-98ea-93d29914e0b3)


Création de la Carte de Disparité

La dernière étape consiste à créer la carte de disparité :

	•	Calcul des disparités : Calcul de la différence de position horizontale entre les points correspondants.
	•	Génération de la carte de disparité : Utilisation des disparités calculées pour créer une représentation visuelle de la profondeur.
![ảnh](https://github.com/user-attachments/assets/9c337246-4f83-4126-b9a8-816bc5bf402d)

Résultats et Analyse
![ảnh](https://github.com/user-attachments/assets/47356478-1749-47bd-8542-a35e26afe59f)

Les résultats montrent les correspondances SIFT détectées et la carte de disparité générée. Nous analysons également la qualité des correspondances en fonction des zones texturées et non texturées des images.

Conclusion

	•	Meilleures correspondances : Se trouvent dans les zones avec des textures distinctes et des caractéristiques uniques.
	•	Moins bonnes correspondances : Se trouvent dans les zones uniformes ou avec peu de détails.

## Contributions

Nous accueillons chaleureusement toutes les contributions. Que vous souhaitiez corriger des bugs, améliorer les modèles ou ajouter de nouvelles fonctionnalités, vos efforts sont les bienvenus. Veuillez soumettre une pull request ou ouvrir une issue pour discuter de vos propositions.

Auteur

Ce projet a été développé par Reagan MANDIYA. Si vous avez des questions ou des suggestions, n’hésitez pas à le contacter.
