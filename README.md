# Application Petclinic

![petclinic](https://miro.medium.com/max/1200/1*f37ndc7_IuuGAsrObp2TNQ.png)

C'est une application pour les cliniques vétérinaires. On retrouve la liste des clients et des praticiens.

## Général

Après plusieurs déploiements en production, l'entreprise en charge de cette application constate des difficultés à maintenir la solution dans Kubernetes.

Par exemple chaque mise à jour de l'application provoque des indisponibilités du service petclinic et la plateforme Kubernetes redémarre les pods sans savoir pourquoi.

Elle fait appel à vous, expert Kubernetes pour les aider dans l'amélioration de leur application.


## Votre mission


Afin d'accompagner cette entreprise dans sa transformation digital et obtenir une application robuste vous aurez besoin de faire :

1- Découper le fichier `petclinic.yml` par type d'objet (Kind) et par composant (nginx, mysql, app)
2- Ajouter les demandes de ressources pour chaque composant (requests) et les limites de consommation (limits)
3- AJouter des sondes pour vérifié l'état Ready des composants (readyness) et vérifié l'état de santé des composants (liveness)
4- Dissimuler le login/password d'accès à la base de donées (secret)
5- Ajouter un accès depuis l'exterieur du cluster kubernetes (ingress)
6- Ajouter de la scalabilité horizontal sur les composants nginx et app (HorizontalPodAutoscaler)
7- Réaliser un package de l'application avec Helm


Pour cela vous allez devoir créer une branche sur le projet git avec votre nom de famille et déployer sur votre branche vos fichiers de YAML.

Créer une branche :

```
git branch -b <nom_de_fammile>
```

Déployer vos fichiers sur votre branche

```
git add -A
git commit -m "Mise à jour des fichiers YAML"
git push
```
