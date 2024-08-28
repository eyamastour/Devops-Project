# Automatisation CI/CD pour l'Application Spring Boot

## <a name="quick-start">🤸 Introduction </a> 
  
   Ce projet vise à mettre en place un pipeline d'automatisation CI/CD pour une application Spring Boot en utilisant divers outils et technologies pour assurer un développement rapide, fiable et de haute qualité.
   Le pipeline comprend des étapes de construction, de tests, d'analyse de code, de gestion des dépendances, de conteneurisation et de surveillance.

## <a name="tech-stack">⚙️ Outils & Technologies Utilisés </a>
  
- GIT : Gestionnaire de version pour suivre les modifications du code source.
- Jenkins : Serveur d'intégration continue pour orchestrer les différentes étapes du pipeline.
- SonarQube : Outil d'analyse de code pour assurer la qualité du code source.
- Nexus : Gestionnaire de dépôts pour stocker les artefacts générés (jar, war, etc.).
- JUnit : Framework de tests unitaires pour valider la fonctionnalité du code.
- Docker : Conteneurisation de l'application pour garantir la cohérence entre les environnements.
- Grafana : Outil de surveillance pour visualiser les métriques et les journaux du système.

  
**Pipeline CI/CD 🔧**

Le pipeline CI/CD est structuré en plusieurs étapes clés :

- Clonage du Dépôt GIT
  Jenkins récupère le code source de l'application depuis le dépôt GIT.

- Compilation du Code
  Utilisation de Maven/Gradle pour compiler le projet Spring Boot.

- Exécution des Tests Unitaires
  JUnit est utilisé pour exécuter les tests unitaires afin de garantir que le code fonctionne comme prévu.

- Analyse de Qualité du Code
  SonarQube analyse le code pour détecter les bugs, les vulnérabilités, et les mauvaises pratiques.

- Gestion des Dépendances et Artefacts
  Les artefacts compilés sont stockés dans Nexus pour une gestion centralisée.

- Conteneurisation avec Docker
  L'application est empaquetée dans une image Docker pour garantir la portabilité et la cohérence entre les environnements.

- Déploiement
  Le déploiement de l'application Dockerisée peut être effectué sur différents environnements (dev, staging, prod).

- Surveillance
  Grafana est utilisé pour surveiller les performances et la santé de l'application en production.

- Configuration et Installation
  
**🔧 Prérequis**
- Jenkins installé et configuré.
- Accès à un serveur GIT pour héberger le code source.
- SonarQube, Nexus, Docker, et Grafana installés et configurés.
  
**Étapes de Configuration**
- Configurer Jenkins : Ajouter un projet Jenkins.
- Configurer le projet pour utiliser le dépôt GIT.
- Ajouter des étapes de build pour compiler, tester, analyser, conteneuriser, et déployer.
- Configurer SonarQube : Configurer le plugin SonarQube dans Jenkins.
- Ajouter les paramètres d'analyse dans le pipeline.
- Configurer Nexus : Configurer Maven/Gradle pour déployer les artefacts dans Nexus.
- Configurer Jenkins pour utiliser Nexus lors du build.
- Configurer Docker : Écrire un Dockerfile pour l'application Spring Boot. / Ajouter des étapes Docker dans le pipeline Jenkins.
- Configurer Grafana : Connecter Grafana à votre source de données pour monitorer les métriques.

**Utilisation**
- Poussez votre code sur le dépôt GIT.
- Jenkins déclenchera automatiquement le pipeline CI/CD.
- Vérifiez chaque étape du pipeline via l'interface Jenkins.
- Les artefacts générés seront disponibles dans Nexus.
- L'application sera déployée et accessible selon la configuration des environnements.
- Utilisez Grafana pour surveiller les performances de l'application.
**Contribuer**
- Pour contribuer à ce projet, veuillez : Cloner le projet.
- Créer une nouvelle branche pour vos modifications (git checkout -b feature/nom-de-la-feature).
- Soumettre une pull request une fois les modifications terminées.
