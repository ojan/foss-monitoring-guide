# Critères d'évaluation

Cette sélection d’outils s’est effectuée en bonne partie à partir de nos retours terrains, de nos retours d’expérience sur des centaines de projets. Nous nous sommes également appuyés sur des évaluations objectives, basées sur 6 critères applicables à toutes les catégories - dont vous trouverez ci-après le détail d’application.

Pour ne pas limiter ce livre blanc à un simple référentiel et en faire un véritable guide pour tous les décideurs, nous avons décidé de publier ces résultats.

Vous disposez ainsi d’indicateurs fiables sur la notoriété de l’outil, sur sa dynamique, sur la qualité de son socle technique, sur son périmètre fonctionnel, sur sa capacité à s’étendre/à s’adapter, et sur la disponibilité de ressources/profils pour vous accompagner dans son intégration à votre environnement.

Lorsque cela était possible, et surtout lorsque cela était pertinent, nous avons déterminé la moyenne des notes par catégorie afin de faire ressortir les points forts et les points faibles de chaque solution.

Vous trouverez ci-dessous le détail des 6 critères d’analyse :

## Notoriété actuelle (en France)

La notoriété actuelle d'une solution est importante dans la mesure où elle est source de sécurité ou au moins de précaution. Cependant, une notoriété construite au moyen d'investissements marketing ne tiendra pas longtemps si elle ne va pas de pair avec une dynamique communautaire et une qualité technique de fond.

S'il est déterminant d'implémenter une bonne solution à l'instant t, il l'est tout autant de s'assurer que les indicateurs sont bien au vert pour que la solution reste bonne dans 3 ans au moins. En effet, disponibilité des ressources, prix et possibilité d’évolutions en dépendront directement. Voilà pourquoi ce critère de notoriété, s'il est important n'est pas suffisant.

Sont considérés:

- Nombre et importance des références client
- Nombre et notoriété des intégrateurs existants (s'agit-il d’indépendants ? de PME ? de grands groupes ? N'y a t-il qu'un seul intégrateur derrière le produit ?)
- Citations dans la presse professionnelle
- Taille des archives des forums et mailing lists
- PageRank Google du site, lié au nombre de sites eux même importants pointant sur le site du produit concerné
- Echanges dans les réseaux sociaux : twitter, facebook, google+, etc .

## Dynamique

Il s'agit de la dynamique autour de la solution, notamment communautaire. Avec la qualité technique, elle va déterminer directement la place de la solution dans le futur. En effet, les investissements d'un éditeur sont finalement peu de choses au regard de tous les correctifs, toute la documentation et même tout le marketing qui peut être fait par une communauté active.

Nous croyons que le modèle dans lequel l'éditeur est pratiquement le seul intégrateur de son produit n’est pas favorable à l’éclosion d’une communauté de partenaires contribuant à la dynamique du produit.

Sont considérés:

- Évolution du volume de forums ou mailing list
- Activité des chats irc
- Gouvernance : dans quelle mesure intégrateurs et utilisateurs sont-ils consultés et partie prenante dans la conception et l'évolution du produit ?
- Fréquence des mises à jour de la documentation, notamment des wiki
- Activité du dépôt de code CVS/SVN
- Fréquence des releases
- Citations par des acteurs indépendants dont les bloggers occasionnels

## Socle technique

Investissements et communauté sont encore peu de chose devant la cohérence, la puissance et l'adéquation avec les standards des modélisations au cœur d’une application open source.

Les fonctionnalités ne sont qu'une surcouche à ces fondations et le coût d'implémentation d'une même fonction métier varie très facilement de 1 à 5 selon la qualité technique des fondations. Ainsi, au delà d'un certain stade, même à grand renforts d'investissements, on ne peut plus enrichir le fonctionnel d’un produit s'il est basé sur des abstractions de trop bas niveau alors qu'une solution bien pensée faite de concepts clairs et efficaces pourra au contraire s'étendre à moindre frais. Bien sûr, un éditeur en bonne santé financière peut recoder sa solution – et c'est courant – mais, vous serez surtout lié à l'ancien produit avec lequel il faudra faire rupture. Si une solution ne peut pas être améliorée de façon continue, c'est vous qui ferez les frais des migrations brutales.

Sont considérés:

- Respect de standards existants (gage de maintenabilité et de facilité de prise en main)
- Puissance et canonicité des abstractions mises en jeu (gage de productivité; sous entendu ici: ORM, webservices natifs...)
- Utilisation d’un framework
- Degré de factorisation du code (gage de fiabilité et de prise en main)
- Habileté des 'hooks', points d'ancrage, et interfaces pour les extensions spécifiques
- Maturité et couverture des webservices
- Courbe d'apprentissage du produit: une courbe plate est moins bien notée
- Modularité de l'application (pattern Inversion Of Control si possible afin que l'application soit composée d'un noyau minimal et de plugins qui sachent bien tenir compte les uns des autres)
- Absence de problème évident de performance

## Périmètre fonctionnel

Il s'agit ici du périmètre fonctionnel global de la solution par rapport à ce que l’on peut couramment trouver parmi les outils de la même catégorie.

Cela offre un indicateur précieux sur la capacité de l’outil ; même si nous nous recommandons, lorsque cela est possible, de descendre au niveau « macroscopique » pour comparer des solutions entre elles sur un périmètre donné. Nos livres thématiques (CMS open source, GED open source, ERP open source, etc.) pourront vous aider.

Précisons également que si ce critère est important pour bénéficier, de base, d’un outil au plus large périmètre possible, le critère de 'souplesse' est autrement plus impactant en termes de coût. En effet sur un outil souple, l'ajout d'une fonctionnalité peut se révéler relativement simple.

## Souplesse / Extensibilité

Dans la mesure où on doit parfois (pour ne pas dire souvent) dépasser le périmètre fonctionnel natif de l'outil, quelle facilité a t-on à le faire? Il s'agit d'un critère déterminant dans le coût total de possession compte-tenu du coût relatif aux éventuels développements spécifiques. La souplesse rejoint ici largement la technologie mais elle met spécifiquement l'accent sur la modularité de l’outil et sur l'efficacité du développement par des parties tierces.

Sont considérés, à titre d’exemples :

- Possibilité d’ajout de plugins
- Facilité à modifier les structures de données pour ajouter ou altérer le stockage des objets métier
- Facilité à modifier les interfaces utilisateur pour leur donner une bonne ergonomie métier
- Facilité à modifier les traitements effectués
- Rapidité, légèreté, des cycles de développement: faut-il recompiler, redéployer des classes, importer ou exporter des méta-données dans la base de données, dès lors comment déploie t-on des adaptations fonctionnelles sur une base de production ?

## Ressources

Difficulté ou non, sur le marché, à mobiliser des prestataires capables d'effectuer des développements pointus sur l'outil. Peut-on trouver facilement des ressources pour mettre en œuvre son projet ? Suis-je dépendant d’un prestataire ?

Attention néanmoins à ne pas mal interpréter cet indicateur car une technologie meilleure peut largement rentabiliser un effort d'adaptation initial supérieur.

## Autres ressources

Autres ressources disponibles pour évaluer des logiciels Open Source

[1](https://fr.wikipedia.org/wiki/M%C3%A9thode_d%27%C3%A9valuation_de_logiciels_libres)
