# Logstash

Logstash est un outil de collecte, analyse et stockage de logs. Il est développé en Java, sous licence Apache 2.0.

Pour la collecte, il sait gérer plus d'une trentaine d'événements. Un événement peut être un message syslog, un mail via le protocole IMAP, un tweet ou encore une commande IRC.

Il va ensuite analyser ces événements, et les mettre en forme à l'aide de filtres. Il existe également une vingtaine de filtres : standardisation de la date, découpage du message, structuration du message via grok.
Après filtrage, on obtient un message relativement clair, avec des couples clé-valeur que l'on pourra exploiter plus tard.

Enfin, il exporte ces données, traitées ou non, sous divers formats : email, sortie standard, fichier texte, alarme Nagios, entrée en base de données ElasticSearch.

Ainsi, on peut très bien traiter plusieurs flux de logs différents, appliquer un filtre à chacun pour harmoniser le tout, et les stocker correctement.

![Fonctionnement de Logstash](https://wooster.checkmy.ws/assets/img/posts/elk-elasticsearch-logstash-kibana/logstash-internal-flow.png)