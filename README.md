# Eaupti

**Plateforme Intelligente d'Agriculture de Précision pour l'Optimisation de l'Irrigation**

*Projet de 3ème année (Module 3pH) - HESTIM*

## À Propos

Eaupti est une plateforme intelligente d'agriculture de précision conçue pour optimiser l'irrigation et les rendements agricoles. En combinant les données de capteurs IoT, l'imagerie satellitaire (Copernicus Sentinel) et les prévisions météorologiques (OpenWeather), la plateforme vise à fournir aux agriculteurs des recommandations d'irrigation exploitables et un tableau de bord multi-parcelles.

*Note : Ce projet est actuellement en phase initiale de configuration et d'analyse.*

## Structure du Dépôt

Ce projet est structuré sous forme de "monorepo" afin de bien séparer les environnements tout en gardant l'ensemble du code au même endroit :

* `/app/web` - Application Front-end (React.js + TypeScript)
* `/services/api` - API Back-end (Python + Flask + PostgreSQL)
* `/packages` - Utilitaires et code partagés (Frontend & Backend)
* `/docs` - Documentation du projet et diagrammes UML

## Pour Commencer

Si vous êtes un membre de l'équipe et que vous souhaitez contribuer au code, **arrêtez-vous ici et lisez d'abord le fichier `CONTRIBUTING.md`.**

Notre dépôt impose des conventions strictes pour le nommage des branches et utilise des outils de contrôle de qualité automatisés (Biome pour TypeScript, Ruff pour Python) via des hooks `pre-commit`. Le guide de contribution vous expliquera étape par étape comment configurer votre environnement local avant de faire votre tout premier commit.
