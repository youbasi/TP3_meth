# Projet : Detection des Fausses Nouvelles
## TP3 : Methodologie pour la science des données
##### Apropos du projet 
Les journaux sont la principale source de nouvelles pour les gens dans le monde entier.
Toutefois, en raison de la croissance importante et des mises à jour des technologies, la
popularité des médias sociaux a augmenté de façon phénoménale. Le nombre de personnes
qui utilisent les médias sociaux a augmenté de façon remarquable, ce qui a eu pour effet
de créer des réseaux sociaux comme les médias sociaux, les sites Web, les blogues, etc.
ont émergé comme des plateformes pertinentes pour recueillir toutes sortes de nouvelles.
Les gens comptent davantage sur les réseaux sociaux que les journaux ces jours-ci. Avec
la disponibilité d’Internet, ces réseaux sont facilement accessibles. Cela peut conduire à
une manipulation facile des nouvelles existantes, provoquant ainsi de fausses nouvelles.
Les fausses nouvelles peuvent être utilisées comme un outil essentiel pour projeter les
gens de la mauvaise façon. Il peut propager la haine parmi les gens, ce qui peut nuire
davantage à la société. Par conséquent, il est très nécessaire d’empêcher la propagation de
fausses nouvelles. Notre projet vise à utiliser diverses méthodes et modèles pour détecter
directement les fausses nouvelles, sur la base du contenu textuel des articles de nouvelles.
Avec l’aide de l’apprentissage automatique ,il est essayé d’agréger les nouvelles et plus
tard déterminer si les nouvelles sont réelles ou fausses en utilisant le classificateur passive agressive,la régression logistique, le classificateur de Decision Tree et on finit avec le classificateur du Random Forest.

### Introduction
Dans l’ère moderne, la diffusion de fausses nouvelles est devenue très évidente. Les
fausses nouvelles sont utilisées à des fins économiques et politiques. La première chose
qui doit être faite pour y parvenir est de détecter les fausses nouvelles. Notre projet
vise à développer un programme d’apprentissage automatique pour identifier quand une
source de nouvelles peut produire de fausses nouvelles. Nous utilisons un corpus d’articles
étiquetés réels et faux pour construire un classificateur qui peut prendre des décisions sur
l’information basée sur le contenu du corpus.

##### Dataset
Le jeu de données que nous utiliserons pour ce projet, nous l’appellerons news.csv qui
est accessible au public pour la classification des fausses nouvelles. Ce jeu de données a
une forme de 7796 *4. Ces déclarations proviennent de facebook, twitter, les sites Web,
les blogues. La première colonne identifie les nouvelles, la deuxième et la troisième sont
le titre et le texte, et la quatrième colonne a des étiquettes indiquant si les nouvelles sont
réelles(REAL) ou fausses(FAKE).
##### Approche proposée
##### Objectif :
L’objectif principal est de détecter les fausses nouvelles, qui est un problème classique
de classification de texte avec une proposition directe. Il est nécessaire de construire un
modèle capable de faire la différence entre les nouvelles réelles et les nouvelles fausses.
 Architecture générale :
Notre système se base sur l’utilisation du Machine Learning pour détecter les Fake
News. Le système prend en entrée une base brute de commentaires et leurs caractéristiques
et la transforme en une base de caractéristiques utilisable par la phase d’apprentissage.
Cette transformation est appelée pré-traitement, elle exécute une série d’opérations telles
que le nettoyage, concaténation. . . . La base pré-traitée est subdivisée en deux parties ;
une pour l’entraînement et l’autre pour le test. Le module d’entraînement utilise la base
d’entraînement et un algorithme d’apprentissage pour fournir un modèle de décision qui
est appliqué sur la base de test. Si le modèle est accepté, c-à-d a pu atteindre un taux de
reconnaissance acceptable, il sera conservé et utilisé par le module d’utilisation et l’entraînement se termine. Dans le cas contraire, les paramètres de l’algorithme d’apprentissage sont révisés dans le but d’améliorer le taux de reconnaissance.
##### Pré-traitement :
Pré-traitement est l’étape pendant laquelle les données brutes sont nettoyées et structurées en vue de l’étape suivante du traitement des données. Dans notre système, on
applique les opérations suivantes
Détecter les valeurs manquantes dans notre jeu de données, et les remplacer par une
chaîne vide, fusionner le titre et le texte dans une seule colonne appelée « content »,
Application d’une fonction qui convertit le texte en minuscules, supprime les espaces
supplémentaires, chr. spécial, ulr et liens, sur la colonne « content », Division de l’ensemble
de données en deux ensembles : ensemble de training et ensemble de tests. X_train :
ensemble de training contenant les caractéristiques Y_train : l’étiquette de l’ensemble de
training X_test : ensemble de test contenant les caractéristiques Y_test : l’étiquette de
l’ensemble de test.
##### Application du modèle d’apprentissage :
C’est la dernière phase de notre système, Après être arrivé au meilleur taux de reconnaissance, ou après avoir construit le modèle dans la phase précédente, nous devons
l’utiliser sur des nouvelles informations non étiquetées, et le modèle nous permet de prédire la classe de la nouvelle si elle est fausse ou vraie avec un degré de confiance.
Dans cette partie nous avons conçu à l’aide de la bibliothèque Tkinter, l’interface utilisateur sous forme de formulaire qui prend comme input le titre et le contenu de la nouvelle,et renvoie, en utilisant le modèle Agressif Passif Classifier, True si la nouvelle est vraie et False si la nouvelle et fausse.
##### Langages et outils utilisés :
-Python 
-JupyterLab
-Pandas
-Scikit-learn
-Re
-Pickle
-Python Imaging Library
-String
-Tkinter
##### Résultats et Évaluation :
Afin d’évaluer nos modèles de classification, et de comparer entre les modèles, nous
avons utilisé l’accuracy.
— Passive Agressive Classifier :77,03%
— Logistic Regression : 81,21%
— Decision Tree :72,62%
— Random Forest Classifier :78%
la Régression Logistique est le modèle que nous a donné la meilleure précision car elle vise à expliquer une variable d’intérêt qui prend uniquement
deux modalités et dans notre cas il s’agit du fake ou real.


##### branches structures
###### - current_code : la parti du code qui n'a pas eté finisilaisé encore et qui peut presenter des erreurs
###### - correct_code : la parti du code qui est correct mais qu'on merge pas encore tant que la parti compléte n'est pas fini
###### - Main : la parti du code 100% fonctionnel et fini 

###### Ce projet a été réalisé par : Oumaima TARHATE & Youssef HAOUES RHAIEM
###### projet universitaire 2022-2023
