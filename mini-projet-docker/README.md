# Hi Legends 👋

# <p align="center">Mini-projet Docker: student list</p>
  
Ce dépot contient une application simple qui utilise un serveur web (PHP) et une API (Flask) pour lister les étudiants. Le projet est empaqueté dans des dconteneurrs Docker pour faciliter le déploiement et la gestion de l'infrastructure.


### Objectifs

- Améliorer le processus de déploiement d'une application existante.
- Gérer le versionnement des releases d'infrastructure.
- Appliquer les meilleures pratiques pour l'implémentation d'infrastructures Docker.
- Infrastructure as Code.
    


### Contexte

POZOS est une entreprise informatique en France qui développe des logiciels pour des établissement scolaires.
L'objectif de ce projet est de construire un POC (Proof of Concept) pour démontrer l'efficacité et la flexibilité de Docker dans la création d'une infrastructure découplée et évolutive.

### Infrastructure

- Utilisation d'une seule machine avec Docker installé pour ce POC.
- Centos 7.6 est le système d'exploitation recommandé pour ce projet.
  

### Application 

Student-list est une application de démonstration composée de deux modules:

1. Une API REST pour envoyer la liste des étudiants en format JSON
2. Une application web en HTML + PHP pour afficher la liste des étudiants
   

### Prérequis 

- Docker et Docker compose doivent être installés sur la machine hôte 
- Les ports nécessaires doivent être ouverts et configurés correctement
  

### Installation et démarrage

1. Cloner le dêpot
2. Exécuter docker - compose up pour construire et lancer les conteneurs
3. Accéder à l'application via un navigateur web ou utiliser des requêtes API pour tester les fonctionnalités
  

### Illustration du projet


![Imgur](https://i.imgur.com/Q2ja7es.png)


### BUILD AND TEST
        
Commande à taper savoir si l'API répond parfaitement:

curl -u toto:python -X GET http://<host IP>:<API exposed port>/pozos/api/v1.0/get_student_ages
(En entrant l'ip du host et le port que vous avez exposé)

Résultat


![Imgur](https://i.imgur.com/YmShKd5.png)


### Infrastructure As code 

Résultat


![Imgur](https://i.imgur.com/reWuSKw.png)


### Docker registry

Résultat


![Imgur](https://i.imgur.com/q5MAVSy.png)


        
        
        
        
    
             
 
    
    
        