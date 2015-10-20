# Heka

Heka est un logiciel de traitement de flux Open Source développé par Mozilla.

Heka se veut être le couteau suisse de la collecte et du traitement de données, utile pour une grande variété de tâches différentes, parmi lesquelles il est possible de citer :

- Chargement et analyse des fichiers journaux à partir d’un système de fichiers.
- Accepter les données en entrée au « format » statsd et les transmettre vers des bases de données de séries chronologiques Graphite ou InfluxDB.
- Lancement de processus externes pour recueillir les données et métriques du système local.
- Analyse en temps réel et détection d’anomalies sur les données circulant à travers le pipeline Heka.
- Envoi de données d’un endroit à un autre par l’intermédiaire d’un transport extérieur (comme AMQP) ou directement (via TCP).
- Fourniture de données traitées à un ou plusieurs puits de données persistantes.

Heka est écrit en langage Go, qui est reconnu comme bien adapté à la construction d’un pipeline de données à la fois souple et rapide. Les tests initiaux montre qu’une simple instance de Heka est capable de recevoir et de router plus de 10 gigabits de messages par seconde ! Ces chiffres impressionnants sont fournis par les développeurs de Heka.

Heka possède un tableau de bord qui présente la particularité d’être mis à jour en temps réel. Les données arrivent, elles sont affichées, pas de navigateur à recharger, y compris pour les graphiques.