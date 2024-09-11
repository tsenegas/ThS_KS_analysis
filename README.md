# Kickstarter dataset Analysis

- [Website](https://tsenegas.github.io/ThS_KS_analysis/)

# Executive Summary

Dans le cadre de cette analyse technique en science des données, j'ai choisi d'utiliser et découvrir le nouvel IDE de Posit (anciennement Rstudio). Ce nouvel IDE offre une intégration fluide entre différents langages de programmation, notamment R et Python mais également Julia ou SQL. En tant qu'utilisateur principal de R, cette approche m'a permis de réaliser l'analyse de manièere rapide en utilisant R tout en fournissant une version de Python au sein du même projet.

J'ai voulu faire l'analyse du jeu de donnée Kickstarter de manière simple et rapide. La réalisation de l'analyse en R a pris environ 2h30. Dans l'analyse en Python, curieux de voir si je pouvais améliorer mon premier modèle réalisé en R, j'ai décidé de tester directement un modèle lightGBM et sélectionné des variables un peu différentes - la traduction basique du code R en Python ne me semblant pas très intéressante.

# R Analysis - EDA & Data Modeling 

- [R Analysis - EDA & Data Modeling](https://tsenegas.github.io/ThS_KS_analysis/R_Analysis.html)

# Python - lightGBM Model

- [Python - lightGBM Model](https://tsenegas.github.io/ThS_KS_analysis/Python_model.html)

# Conclusion

En nous limitant à des modèles simples incluant très peu de variables, nous obtenons des résultats encourageants. Nous pouvons réfléchir à ajouter de nouvelles variables pour augmenter l'efficacité de nos modèles.

La prochaine étape est de déployer notre modèle, soit dans une API, soit dans une application web, permettant au client de tester la probabilité de réussite de son projet.

Comme tout modèle, le nôtre va voir sa performance fluctuer avec le temps. Il est donc important de réentraîner notre modèle constamment et de faire un suivi de celui-ci (MLOps). Il serait également préférable de faire tourner plusieurs modèles afin de pouvoir surveiller les différentes métriques. Le modèle le plus performant sera celui accessible via l'API et/ou l'application web.

Nous pourrions facilement intégrer un modèle d'IA générative pour proposer des suggestions de noms de projets afin d'augmenter le taux de probabilité de réussite de celui-ci.

# Set-up

Voici l'installation réalisé pour reproduire dans les même conditions

- Platform: x86_64-w64-mingw32/x64
- Running under: Windows 11 x64 (build 22631)

- Install R version 4.4.1 - [Install R 4.4.1](https://cran.r-project.org/bin/windows/base/)
- Install Python 3.12.16 - [Install Python 3.12.16](https://www.python.org/downloads/release/python-3120/)
- Install the latest Visual C++ Redistributable - [Windows Visual C++ Redistributable Version](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170#latest-microsoft-visual-c-redistributable-version)
- Install Positron IDE - [Positron](https://github.com/posit-dev/positron/releases)
