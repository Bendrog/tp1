# Answers

Nom : Drogou 
Prénom : Benoit

# 1.
**Qu'est-ce qu'une instance EC2 ?**

> Elastic Compute Cloud (EC2) est utilisé par AWS pour héberger des serveurs virtuels.

# 2.
**Qu'est-ce qu'un VPC ?**

> Un Virtual Private Cloud est présent dans un environnement de cloud public. Il délivre une connexion indépendante et sécurisée entre les utilisateurs et leurs instances. Par exemple, le produit Amazon Virtual Private Cloud (AVPC) permet aux utilisateurs d'obtenir une section du réseau AWS.

# 3.
**A quoi sert un NSG ?**

> Un Network Security Group (NSG) joue le rôle d'un firewall pour les Machines Virtuelles. Il est composé des règles qui permettent de déterminer les communications autorisées entre la VM et internet. Tant en sortie ou en entrée de la VM

# 4.
**Quelles sont les 5 propriétés désirables du cloud ?**

1. **_Le paiement à l'usage_**: On ne paie que ce que l'on consomme.
2. **_Elastique_**: Le cloud offre la possibilité d'adapter le nombre de serveur selon la demande. Ce qui permet une scalabilitée rapide.
3. **_Ouvert_**: Disponible avec une conection internet, ouvert sur le monde.
4. **_Mutaliser_**: Les services de coud proposent un ensemble de ressources dématéralisées accessibles par tous les utilisateurs. Elles sont paratgées. De ce fait, les entreprises ne sont plus obligées d'investir dans du hardware et d'en assurer la maintenance.
5. **_Libre-Service_** : Beaucoup de stack, d'outils open-sources. 

# 5.
**Qu'est-ce que l'A/B Testing ?**

> L' A/B testing est une méthode, souvent utilisée dans le marketing visant à étudier l'action d'un utilisateurs afin d'améliorer l'UX d'un produit. Le principe étant de divier une population en 2 catégories A et B (Il faut que la séparation soit faite le plus aléatoirement possible, sans pattern entre les 2 groupe: ages, sexe, corps de métiers etc...). Puis assigner un visuel légerement différent pour les 2 groupes. En analysant les comportement des utilisateurs on peut déterminer laquelle des versions du produit est la plus efficace pour un comportement donné. 

# 6.
**Comment programmer le cloud ?**
> L'Infrastructure as Code (IaC) est une solution qui permet de gérer la structure des machines, disposées dans la cloud, à partir de la lecture d'un "simple" fichier. Que ce soit le choix de l'OS de la machine ou les différentes application à y installer. Un gain de temps comparer à faire ce process manuellement en ligne de commande.

# 7.
**Quelle est la technique pour faire un déploiement sans interruption de service ?**

> Le Zero Downtime Deployment (ZDD) permet de déployer une nouvelle version d'un système tout en sans intérompre le service. Le Blue/Green Deployment, le Canary Release et le Dark Launch sont différente variantes exploitant cette technique

# 8.
**Qu'est-ce que le Canary release ?**

> Le Canary release est un technique de ZDD qui a pour but de simplement mettre une petite portion d'utilisateurs sur le version N+1 (5%). Puis, si aucun problème n'est détecté, progressivement augmenter le volume d'utilisateurs sur cette nouvelle version jusq'à atteindre les 100% d'utilisateurs. Il y a donc les 2 versions N et N+1 en même temps en production.

# 9.
**Comment changer de taille de machine virtuelle ?**
> Il y a une interface graphique sur le provider, Amazon Web Service par exemple. Il suiffit de manuellement augmenter la taille de sa Machine Virtuelle et automatiquement l'infrastructure est modifiée (et le billing aussi .... $$).
On va dans les paramètres de la machine et on augmente simplement la taille que l'on souhaite attribuer. le cloud se charge du reste

# 10.
**Qu'est-ce que le Blue/Green deployment ?**

> Le principe du Blue/Green deployment est de basculer les utilisateurs vers la nouvelle version (N+1; Green) tout en maintenant le version précédente (N; Blue) sur une autre branche. Si un problème survient, le rollback est très facile. Il suffit de rebasculer le traffic vers la branche de la version N.
