---

# Prédiction de la Valeur Vie Client (CLV) & Segmentation par LTV

### Objectif :

Nous devons prédire la valeur vie du client (Customer Lifetime Value - CLV) et segmenter les clients selon leur LTV afin de fournir ces informations à l’équipe marketing pour optimiser les campagnes et le coût par acquisition (CPA).

### Introduction :

Le jeu de données utilisé pour ce projet provient du **UCI Machine Learning Repository**. Il s’agit de données transactionnelles issues d’un site e-commerce britannique. L’entreprise vend principalement des cadeaux uniques pour toutes occasions. Le dataset comprend plusieurs variables : numéro de facture, code produit, description, quantité, date de la commande, prix unitaire, ID client, etc.

Avant de commencer la modélisation, comprenons d'abord ce qu’est la **valeur vie client (CLV)**.

![Prédiction de la Valeur Vie Client](https://neilpatel.com/wp-content/uploads/2018/05/facebook-lifetime-value.jpg)

### Résumé

**Qu’est-ce que la Valeur Vie Client (CLV) ?**

La [valeur vie client (CLV)](https://fr.wikipedia.org/wiki/Valeur_vie_client) est une statistique essentielle dans le cadre d’un programme d’expérience client. Elle mesure la valeur qu’un client représente pour une entreprise sur toute la durée de leur relation, et non seulement lors du premier achat. Cette métrique permet de comprendre le coût raisonnable d’acquisition d’un client.

Le CLV représente donc la valeur totale qu’un client apporte à une entreprise pendant toute la durée de leur relation. C’est un indicateur clé car fidéliser un client existant coûte généralement moins cher que d’en acquérir un nouveau. Augmenter la valeur des clients existants est donc un levier important de croissance.

**Défis —**
Certaines entreprises ne tentent même pas d’estimer le CLV en raison de la fragmentation des équipes, des systèmes inadéquats ou d’un marketing peu ciblé.

**Pourquoi est-il important de suivre le CLV ?**

Le CLV aide les marketeurs à estimer le chiffre d'affaires potentiel qu’un client peut générer tout au long de sa relation avec l’entreprise. Plus cette relation dure, plus la valeur client augmente.

Pour calculer le CLV, plusieurs méthodes existent en ligne, mais ici, je vais vous présenter le modèle que j’ai choisi et les raisons de ce choix.

Avant de modéliser, il est crucial de comprendre le **contexte business** ainsi que les comportements des clients.

Il existe deux grands types de contextes commerciaux, en fonction de la relation client et des opportunités d’achat :

**a) Contractuel —** Ici, on sait précisément quand un client va partir. Ce type de relation est appelé *contractuelle*, et les clients sont dits *abonnés*.
Exemples : Hotstar, Netflix, Amazon Prime.

**b) Non-Contractuel —** Les clients partent silencieusement, sans avertissement. Cela rend le calcul du CLV plus complexe.
Exemples : Retail / E-commerce.

![Contexte Business](https://2zzm8x3dsugfsdli13ukukea-wpengine.netdna-ssl.com/wp-content/uploads/hardie_non_contract_continuous.png)

**Types d’opportunités d’achat :**

**a) Continue —** Les achats peuvent avoir lieu à tout moment.

**b) Discrète —** Les achats se font à intervalles définis.
Exemple : Plans d’abonnement.

Selon ce cadre, on peut identifier le bon contexte et choisir la méthode la plus adaptée.

### Objectif de l’étude

Suite au problème et à la motivation évoqués ci-dessus, cette étude vise à explorer différentes méthodes adaptées au contexte *non-contractuel et continu* pour estimer les revenus potentiels (CLV) générés par un groupe de clients actifs.

Pour cette estimation, des **modèles probabilistes** (Pareto-NBD, BG-NBD, MBG-NBD et Gamma-Gamma) ont été appliqués à une étude de cas dans le secteur. Une **segmentation client par apprentissage non supervisé** a également été effectuée pour démontrer un outil efficace de planification stratégique.

***Étapes du projet :***
Importation des données | Nettoyage des données | Analyse exploratoire | Ingénierie des caractéristiques | Validation croisée | Modélisation prédictive | Segmentation LTV | Évaluation du modèle | Déploiement

***Bibliothèques utilisées :***

a) Scikit-learn
b) Lifetimes
c) Plotly, Matplotlib, Seaborn, Altair
d) XLRD
e) Streamlit
f) Numpy
g) Pandas
h) Datetime
i) Math
j) Pickle
k) Warnings
l) Streamlit (répété par erreur dans l'original)

**Hébergement & Déploiement du modèle :** Heroku | GitHub | Streamlit
---

