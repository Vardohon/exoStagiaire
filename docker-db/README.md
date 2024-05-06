# Modèle Docker pour BDD MariaDB

Ces fichiers de configuration peuvent servir de base pour la création d'un conteneur de SGBD MariaDB.

Pensez à modifier les variables d'environnement contenues dans le fichier `.env` :
- `MARIADB_DATABASE` ;
- `MARIADB_USER` ;
- `MARIADB_PASSWORD` ;
- `MARIADB_ROOT_PASSWORD`.

Ajoutez vos scripts sql dans le sous dossier `db/dump`.

> [!IMPORTANT]
> Il n'est pas nécessaire d'ajouter les commandes `create database` et `use database` au script de création.

Pour lancer la base de données :
```bash
docker compose up
```


