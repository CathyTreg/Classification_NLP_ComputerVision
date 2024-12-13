# Classification_NLP_ComputerVision
Catégoriser les articles d’une marketplace avec leur image et leur description - Projet réalisé en juin 2024 dans le cadre du parcours de formation DataScientist d'OpenClassrooms.

Contexte : L’entreprise "Place de marché" lance une marketplace e-commerce où les vendeurs publient des produits accompagnés d'une photo et d'une description. L’entreprise voudrait automatiser le processus de catégorisation des articles en fonction de leur description où de leur image.
Objectif : Créer un moteur de classification automatique des produits basé sur leur description ou leur image, afin d’optimiser la gestion des produits sur la marketplace.

Tâches :
-	Traitement des descriptions (NLP) :
    - tester plusieurs modèles sur les descriptions (TF-IDF, Word2Vec, BERT) pour étudier la faisabilité de regrouper les articles de même catégorie en fonction de leur descriptif.
-	Traitement des images (Computer Vision) :
    - tester plusieurs modèles de traitement des images (SIFT, CNN) pour étudier la faisabilité de regrouper les articles de même catégorie en fonction de leur image ;
    - appliquer le modèle de classification supervisée avec un réseau de neurones convolutifs (CNN) pour classer les produits en fonction de leurs images. Le modèle pré-entraîné VGG16 a été utilisé, avec des techniques d’augmentation des données pour améliorer la robustesse du modèle.
-	Exploration de nouvelles techniques :
    - étudier et mettre en œuvre le modèle Vision Transformer (ViT), une approche récente en Computer Vision, pour challenger la méthode CNN. Le modèle pré-entraîné ViT a été affiné avec les données de ImageNet et comparé à l'approche CNN en termes de performance.

Résultats : 
-	Classification via descriptions : l'approche TF-IDF a permis d'obtenir des résultats satisfaisants pour la catégorisation des produits, facilitant l'automatisation du processus.
-	Classification via images : l’utilisation du modèle CNN pré-entraîné VGG16 a permis de classer correctement plus de 80% des images, montrant que les réseaux de neurones sont efficaces pour cette tâche.
-	Comparaison des modèles : la comparaison entre CNN et ViT a révélé que ViT peut offrir de meilleures performances dans certaines catégories de produits, notamment pour des images plus complexes et diversifiées.

Environnement de travail : Jupyter Notebook - Python (via Anaconda), Google Collab
Librairies : Numpy – Pandas – Matplotlib – Seaborn – Scikit-learn – NLTK – Spacy – Tensorflow – Keras – Transformers (HuggingFace) – Torch (PyTorch)
