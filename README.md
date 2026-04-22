# projet_docker-Carbet_Eddy #


# POUR CONSTRUIRE L'IMAGE #
**1.** Ouvrir le terminal à la racine du projet où se trouve le docker-compose.yml </br>
**2.** Lancer la commande : 'docker compose up -d' </br>

# POUR DESCENDRE L'IMAGE #
**1.** Ouvrir le terminal à la racine du projet où se trouve le docker-compose.yml </br>
**2.** Lance la commande : 'docker compose down' (utilisez le flag -v en fin de commande pour supprimer les volumes) </br>

# PORTS D'ACCES AUX SERVICES ##
**MAILHOG :** 8025:8025 </br>
**APP (Interface utilisateur) :** 8080:80 </br>
**PHPMYADMIN :** 8081:81 </br>
**MYSQL (BD) :** 3306:3306 </br>

# POUR RESTAURER UNE BASE DE DONNEE #
**1.** Ouvrir le terminal à la racine du projet à la racine du dossier </br>
**2.** Placer votre fichier contenant le script de construction de BDD dans ./sql </br>
**2.** lancer la commande : mysql -h 127.0.0.1 -p 3306 -u bloguser -pblogpass << ./sql/ votreFichierAveclaBDD.sql </br>
