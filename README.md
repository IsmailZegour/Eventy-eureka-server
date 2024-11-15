# Eventy - Serveur Eureka

Bienvenue dans le projet Eventy! Ce dépôt contient la configuration pour le serveur Eureka de l'application Eventy, qui centralise l'enregistrement et la découverte des microservices utilisés par l'application. En utilisant Eureka comme registre de services, nous assurons que tous les microservices de l'application peuvent être découverts et communiquent facilement entre eux.

## Table des matières
- [Aperçu du Projet](#aperçu-du-projet)
- [Prérequis](#prérequis)
- [Installation et Démarrage](#installation-et-démarrage)
- [Configuration](#configuration)
- [Utilisation](#utilisation)
- [Dépannage](#dépannage)
- [Contribuer](#contribuer)
- [Licence](#licence)

## Aperçu du Projet

Le serveur Eureka est un service de registre centralisé pour les microservices de l'application Eventy. Chaque microservice de l'écosystème Eventy se connecte à ce serveur Eureka pour :
- S'enregistrer automatiquement,
- Découvrir les autres services disponibles,
- Assurer une résilience et une disponibilité accrues en gérant le routage des appels entre services.

**Fonctionnalités principales :**
- Enregistrement et découverte de services,
- Tableau de bord pour surveiller les instances de services enregistrées,
- Load balancing rudimentaire pour répartir les requêtes entre les instances de microservices.

## Prérequis

- **Java** 11 ou supérieur
- **Maven** 3.6+
- **Spring Boot** 2.6+
- Accès à un environnement de réseau commun pour permettre aux microservices de communiquer avec Eureka.

## Installation et Démarrage

### Cloner le dépôt
Clonez ce dépôt sur votre machine locale :
```bash
git clone https://github.com/votre-utilisateur/eventy-eureka-server.git
cd eventy-eureka-server
