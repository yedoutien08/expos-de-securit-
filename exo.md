 # **exposé sur la sécurité**

## les types d'attaques

* Attaques par déni de service (DoS) et par déni de service distribué (DDoS)
* Attaque de l’homme au milieu (MitM)
* Hameçonnage (phishing) et harponnage (spear phishing)
* Téléchargement furtif (drive-by download)
* Cassage de mot de passe
* Injection SQL
* Cross-site scripting (XSS)
* Écoute clandestine
* Attaque des anniversaires
* Logiciel malveillant (malware)


## les attaques qui se rapproche a une base de donnée

Une liste des principaux types d'attaques sur les bases de données peuvent être classées comme:

* Une mauvaise presse de information;
* Modifier des données incorrectes;
* Déni de service.
Ces trois grandes catégories sont donc en étroite harmonie avec les atteintes à la confidentialité, l'intégrité et la confidentialité mentionnées.

## lieu de stockage et les extensions des bases de donneé

## cas de oracle
* ### cles extensions
Les fichiers d'une base de données Oracle sont les suivants :

1. Les fichiers de données (dont l'extension est .dbf). Ces fichiers contiennent l'ensemble des données de la base (les tables, les vues, les procédures stockées, ...).
2. Les fichiers Redo Log (dont l'extension est .rdo ou .log). Ces fichiers contiennent l'historique des modifications effectuées sur la base de données
3. Les fichiers de contrôle (dont l'extension est .ctl).
 Ces fichiers permettent de stocker les informations sur l'état de la base de données (emplacement des fichiers, dates de création, ...)


* ### lieu de stockage
 Les sauvegardes sont stockées dans OCI Object Storage. Object Storage a été conçu pour être extrêmement durable. Les données sont stockées de manière redondante sur plusieurs serveurs de stockage et dans plusieurs domaines de disponibilité.

## cas de mysql

* ### les extension

Extensions reliées à SQL:
1. dbf Aston-Tate dBASE Database
2. sqr SQR Script
3. gdb Embarcadero InterBase Database File
4. rbf RBase Data
5. db General Database File
6. spf SQR Portable Format
7. lis SQR Printer Output
8. mkd Pervasive SQL Database
9. sqs SQL Script Sequences
10. con SQL Script Constraints

* ### lieu de stockage

Présentation. Par défaut, les bases de données (en tant que fichier) sont stockées dans "/var/lib/mysql/" sous Linux. Pour des questions d'organisation, de sécurité ou de place, il est peut être intéressant de changer l'emplacement de ces bases de données vers un autre dossier/ chemin.


## cas de postgres
* ## les extension

pgsql est l'inxtension de postgres
Extensions associées:
1. dbf Base de données Aston-Tate dBASE
2. sqr Script SQR
3. sql Script SQL
4. gdb Fichier de base de données Embarcadero InterBase
5. rbf Données RBase
6. db Fichier de base de données général
7. spf Format portable SQR
8. lis Sortie d'imprimante SQR
9. mkd Base de données SQL omniprésente

* ## lieu de stockage
Traditionnellement, les fichiers de configuration et les fichiers de données utilisés par une instance du serveur sont stockés ensemble dans le répertoire des données, habituellement référencé en tant que PGDATA (d'après le nom de la variable d'environnement qui peut être utilisé pour le définir). Un emplacement courant pour PGDATA est /var/lib/pgsql/data. Plusieurs groupes, gérés par différentes instances du serveur, peuvent exister sur la même machine.

Le répertoire PGDATA contient plusieurs sous-répertoires et fichiers de contrôle, comme indiqué dans le Tableau 65.1, « Contenu de PGDATA ».