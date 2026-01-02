# TP 24 – Conteneurisation d’une application Spring Boot & Angular

## Présentation

Ce TP a pour objectif de conteneuriser une application Smart Home développée avec :

- Backend : Spring Boot (Java)

- Frontend : Angular

- Base de données : MySQL en utilisant Docker et Docker Compose.

L’application est déployée sous forme de micro-environnement composé de plusieurs conteneurs communiquant entre eux.

## Architecture :

┌─────────────┐      ┌──────────────┐
│  Frontend   │ ---> │   Backend    │ ---> │ MySQL │
│  (Angular)  │      │ (Spring Boot)│
└─────────────┘      └──────────────┘
                           |
                           v
                    ┌────────────┐
                    │ phpMyAdmin │
                    └────────────┘

## Accès aux services

| Service             | URL                                            |
| ------------------- | ---------------------------------------------- |
| Frontend Angular    | [http://localhost](http://localhost)           |
| Backend Spring Boot | [http://localhost:8085](http://localhost:8085) |
| phpMyAdmin          | [http://localhost:8081](http://localhost:8081) |
| MySQL               | localhost:3306                                 |



- Identifiants MySQL :

       Utilisateur : root

       Mot de passe : root

## Vidéo de démonstration :

  

https://github.com/user-attachments/assets/c30fb950-0474-40b4-b993-721adeea9473


## Objectifs atteints

- Conteneurisation du backend Spring Boot

- Conteneurisation du frontend Angular

- Base de données MySQL en conteneur

- Orchestration avec Docker Compose

- Accès web via Nginx et phpMyAdmin

## Conclusion

Ce TP permet de déployer une application full-stack Spring + Angular de manière portable, reproductible et isolée grâce à Docker.
Il illustre une approche professionnelle de déploiement moderne utilisée en entreprise.
