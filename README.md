# Ultrasound-imaging-classifications-of-Thyroid-nodules

Application de l'apprentissage profond par transfert en imagerie médicale pour l'aide au diagnostic des lésions thyroïdiennes

Résumé

Dans ce travail, nous visons à évaluer et comparer les performances de plusieurs 
architectures CNN pour classer les nodules thyroïdiens en deux classes (malin/bénin) sur des 
images échographiques. A cette fin, nous avons utilisé une base d'images d'une petite taille, 
composée de 269 cas de lésions bénignes et 526 cas de lésions malignes. Afin de compenser 
le manque de volume de cette base, le transfert d'apprentissage est appliqué d’une manière 
progressive sur trois modèles CNN existants (VGG-16, ResNet-50 et EfficientNet). Ces 
derniers sont pré-entrainés, en premier lieu, sur la base d'images ImageNet (disponible en 
grande taille mais de nature très différente de notre base d'images), et en second lieu, sur une 
base d'images radiographiques qui concerne une autre maladie (disponible en taille moyenne 
avec une nature proche à notre base). Ces modèles sont affinés selon différents niveaux et 
stratégies de fine-tuning. Pour la classification des lésions en maligne ou bénigne, nous avons 
utilisé un classifieur softmax supervisé sur les trois modèles, à l’exception du modèle VGG16, où nous avons testé deux autres classifieurs supplémentaires, le SVM et le Random 
Forest. Les résultats obtenus montrent la possibilité de passer facilement de la classification 
d'une maladie vers une autre qui dispose d'un nombre d'images limité en profitant des 
connaissances déjà acquises sur une autres base très large.

Mots-clés : Système d'aide au diagnostic médical, apprentissage profond, vision par 
ordinateur, intelligence artificielle.

Abstract

In this master’s project, we aim to evaluate and compare the performance of several 
CNN architectures to classify thyroid nodules into two classes (malignant / benign) on 
ultrasound images. To this end, we used a small base of images, made up of 269 cases of 
benign lesions and 526 cases of malignant lesions. In order to compensate for the lack of 
volume of this base, the transfer learning is applied in a progressive way on three existing 
CNN models (VGG-16, ResNet-50 and EfficientNet). The latter are pre-trained, firstly, on the 
database ImageNet (available in large size but of a very different nature from our image 
database), and secondly, on a database of radiographic images which concerns another disease 
(available in medium size with a nature close to our base). These models are refined 
according to different levels and fine-tuning strategies. For the classification of lesions as 
malignant or benign, we used a supervised softmax classifier on all three models, with the 
exception of the VGG-16 model, where we tested two other additional classifiers, the SVM 
and the Random Forest. The results obtained show the possibility of easily passing from the 
classification of a disease to another which has a limited number of images by taking 
advantage of the knowledge already acquired on a very large database.

Keywords: computer-aided diagnosis system in medical imaging, deep learning, computer 
vision, artificial intelligence.

  Pour l’implémentation du système, plusieurs bibliothèques et technologies ont été 
nécessaires :

Plateforme TensorFlow, Keras  

Environnements virtuels dans Jupyter Notebook : Google Colab, Jupyter Notebook

Gradio : Interfaces graphiques pour les modèles de ML et DL

