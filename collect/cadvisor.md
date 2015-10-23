# Cadvisor

cAdvisor (Container Advisor) fournit aux utilisateurs de conteneurs un outil pour comprendre l'utilisation des ressources et les caractéristiques de performance de leurs conteneurs en fonctionnement.

C'est un démon qui recueille, agrège, traite et exporte les  informations des conteneurs en cours d'exécution. Pour chaque conteneur, il conserve les paramètres d'isolation des ressources, un historique de l'utilisation des ressources, des histogrammes de statistiques historiques complets d'utilisation des ressources et du réseau. Ces données sont exportées par conteneur pour l'ensemble du serveur de conteneurs.

cAdvisor a un support natif pour les conteneurs Docker et devrait pouvoir fonctionner avec à peu près tout autres types de systèmes.