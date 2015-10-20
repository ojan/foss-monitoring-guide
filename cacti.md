# Cacti

Cacti est un outil basé sur RRDTool dédié à la métrologie. Il permet de représenter sous forme de graphiques n'importe quelle donnée quantifiable collectée soit par le biais de protocoles réseaux tels que SNMP ou soit par des scripts personnalisés par l'utilisateur.

Il est considéré comme étant le digne successeur de MRTG et apporte une véritable interface à RRDTool en permettant de modifier chacun des aspects des graphiques générés. Les possibilités de configuration très avancées font que celui-ci est souvent utilisé en complément de solutions de supervision tel que Nagios, notamment, pour assurer la partie métrologie lorsque les exigences sont fortes.

De nombreux plugins développés par la communauté permettent d'étendre les fonctionnalités de Cacti et parfois bien même au delà de la simple métrologie. Cacti est distribué sous la licence GPL v2.

Il fonctionne grâce à un serveur web équipé d'une base de données et du langage PHP. Cacti utilise aussi un système de scripts (Bash, PHP, Perl, VBs...) pour effectuer des mesures plus complexes.
