# Classification_NLP_ComputerVision
Catégoriser les articles d’une marketplace avec leur image et leur description - Projet réalisé en juin 2024 dans le cadre du parcours de formation DataScientist d'OpenClassrooms.

Contexte : 
-	L’entreprise "Place de marché” lance une marketplace e-commerce.
-	Les vendeurs proposent des articles de différentes catégories en postant une photo et une description. Les catégories sont définies manuellement.
-	Pour permettre le déploiement de la marketplace, il est nécessaire d’automatiser le process de catégorisation des produits.

Tâche :
-	Elaborer un modèle de classification des articles (avec sa description ou son image) qui permettra de labéliser automatiquement les articles à partir des informations postées par le vendeur.

Actions : 
-	Réaliser un traitement NLP sur les descriptions pour étudier la faisabilité de regrouper les articles de même catégorie en fonction de leur descriptif : montrer via une classification non supervisée qu’il est réalisable de séparer automatiquement les produits selon leur vraie classe avant de faire la classification supervisée (plus lourde).
-	Réaliser un traitement des images (Computer Vision) pour étudier la faisabilité de regrouper les articles de même catégorie en fonction de leur image.
-	Réaliser la classification supervisée avec la méthode identifiée (Classification CNN).
-	Etudier une technique récente de classification d’images (Vision Transformer) pour challenger la méthode mise en place. Réaliser un état de l’art sur la technique, l’implémenter et la comparer à l’approche précédente.

Résultats : 
-	La création d’un moteur de classification est possible via les descriptions et les images.
-	Catégorisation via les descriptions : l’approche TF-IDF donne de bons résultats et est facile à mettre en place.
-	Catégorisation via les images : il est nécessaire de passer par un modèle pré-entrainé utilisant des réseaux de neurones pour classer les images car une approche plus simple n’est pas concluante. Plus de 80% des images sont bien catégorisées avec le modèle CNN mis en place. 
-	Livraison d’une note méthodologique comparant les méthodes : CNN avec Data Augmentation (modèle VGG16 pré-entraîné sur la base de données ImageNet) et Vision Transformer avec Data Augmentation (modèle ViT pré-entraîné sur ImageNet-21k et affiné sur ImageNet-2012).

Environnement de travail : Jupyter Notebook - Python (via Anaconda), Google Collab
Librairies : Numpy – Pandas – Matplotlib – Seaborn – Scikit-learn – NLTK – Spacy – Tensorflow – Keras – Transformers (HuggingFace) – Torch (PyTorch)
