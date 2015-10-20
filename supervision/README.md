# Supervision

La supervision est un sujet présent dans tous les systèmes d’information à partir d’une certaine taille. Alors que certains préfèrent des outils libres tels que Nagios, Nagvis, Shinken ou Icinga, d’autres utilisent des solutions propriétaires, souvent plus simple d’accès et d’administration tel que PRTG. On oublie cependant parfois que la “supervision” n’est qu’un des éléments qui composent le monitoring.

Le monitoring (ou monitorage en français, mais on gardera monitoring 😉 ), désigne le fait de “surveiller” , ou “garder un oeil sur” . Cependant, le fait de surveiller quelque chose revient à connaître sont état actuel mais aussi l’historique de ses états passés, par l’intermédiaire de valeurs (UP/DOWN) et de données chiffrées (des pourcentages par exemple). C’est ici que l’on retrouve une distinction entre deux notions que sont la supervision et la métrologie.

La métrologie, dans laquelle on retrouve la notion de mètre/métrique, est le fait d’obtenir, de garder et de tracer la valeur numérique d’une charge. Par exemple le pourcentage de CPU utilisé sur un serveur, le nombre de personnes connectées sur une site web, le trafic sortant et entrant sur un switch. Bien souvent, la métrologie permet tout simplement de tracer des graphiques, bien connus dans le domaine du monitoring :
cacti-exemple-monitoring-01

Exemple de graphiques produits par Cacti/Munin (RDDTOOL). Ici, aucune indication concernant l’état à l’instant T mais un historique de valeurs numériques retraçant l’évolution d’une charge.

La métrologie est donc le fait de récupérer la charge (chiffrée), permettant de tracer son évolution dans le temps. Elle est donc caractérisée non pas par le fait de récupérer une valeur à l’instant T, mais de pouvoir afficher et tracer l’évolution d’une charge, construite par un ensemble de métrique récupérées dans le temps.

La supervision, en revanche, est le fait de récupérer l’état d’un service à l’instant T. la supervision vise à répondre à la question “Le service est-il joignable ?” . Au sens strict du terme, aucune valeur numérique n’entre en compte, et l’aspect historique de charge ne fait donc pas partie de la supervision. L’exemple le plus frappant est Nagios qui, par défaut, ne possède aucune fonctionnalité permettant de tracer des graphiques ou obtenir l’historique de la charge d’un service/serveur. Une “extension” de la supervision porte sur le fait de récupérer une valeur chiffrée comme une charge mémoire et de lui appliquer un seuil d’alerte. Dans ce cas, aucun historique n’est gardé mais l’on est capable d’obtenir et de surveiller non plus des états, mais des valeurs numériques.
nagios-exemple-monitoring-01

Ici, on voit un exemple de la page Nagios rapportant les états de différents services (OK, CRITICAL, etc.)

La supervision se caractérise d’ailleurs aussi par son système d’alerte, conséquence directe de la vision “à l’instant T”. On peut alors avertir l’administrateur si un système passe de UP à DOWN et inversement. Au contraire, dans le concept pure de la métrologie, le système d’alerte n’est pas pris en compte car la récupération des valeurs/charges n’est pas forcément faite à l’instant T.

À l’inverse de Nagios, des solutions comme Munin ou Cacti ne possèdent aucune fonctionnalité permettant de connaître l’état (UP/DOWN) d’un service à l’instant T, mais sont capables de tracer un ensemble de graphiques afin de retracer la charge de différents services/serveurs et de leur ressources.

Et oui ! Munin et Cacti ne sont pas des outils de supervision mais des outils de métrologie ! Cacti permet seulement, grâce à une extension, d’émettre des alertes sur les valeurs numériques récupérées, c’est là toute la différence entre métrologie et supervision !

Avec le temps, supervision et métrologie tendent à complètement se confondre dans les solutions proposées. Ainsi, lorsque l’on cherche à récupérer une information, on parle alors de monitoring. On est maintenant capable d’appliquer de la supervision sur la métrologie, pour faire plus claire, on va appliquer des alertes sur des seuils de charge. Certains produits permettent d’ailleurs de fusionner totalement métrologie et supervision dans le sens où, si la charge (par exemple CPU) est très différente de l’historique habituel des 7 derniers jours, alors on envoie une alerte.

D’autres solutions permettent même d’établir une prévision de charge en utilisant les données métriques récupérées (l’historique de charge), puis d’y appliquer un processus de supervision permettant de vérifier si la charge en cours est cohérente avec la charge prévue, alertant l’administrateur en cas de forte différence.

Bref ! Le sujet est vaste et les notions de supervision et métrologie tendent de plus en plus à se confondre. Le terme monitoring quant à lui englobe les deux concepts.

Sélection_005Nombreux sont les informaticiens, même expérimentés, ne faisant pas la distinction, certains croyaient même que je faisais une mauvaise blague lorsque je leur expliquais la différence entre monitoring, supervision et métrologie. Et vous, faites vous la différence entre les concepts de métrologie/supervision ?