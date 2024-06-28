# Sequelize Migrations et Seeds

Ce projet utilise Sequelize pour gérer les migrations et les seeds de la base de données.

## Création du premier modèle (et migration)

Pour créer votre premier modèle et migration, utilisez la commande suivante :

```bash
npx sequelize-cli model:generate --name User --attributes firstName:string,lastName:string,email:string
```

## Exécution des migrations
Pour exécuter toutes les migrations disponibles, utilisez la commande suivante :

```bash
npx sequelize-cli db:migrate
```

## Annulation des migrations
Pour annuler la dernière migration exécutée, utilisez la commande suivante :
```bash
npx sequelize-cli db:migrate:undo
```
Pour annuler toutes les migrations, utilisez la commande suivante :

```bash
npx sequelize-cli db:migrate:undo:all
```

## Création du premier Seed
Pour créer votre premier seed, utilisez la commande suivante :
```bash
npx sequelize-cli seed:generate --name demo-user
```
Cette commande générera un nouveau seed dans seeders/XXXXXX-demo-user.js.


## Exécution des seeds
Pour exécuter tous les seeds disponibles, utilisez la commande suivante :
```bash
npx sequelize-cli db:seed:all
```

Annulation des seeds
Pour annuler le dernier seed exécuté, utilisez la commande suivante :
```bash
npx sequelize-cli db:seed:undo
```
Pour annuler tous les seeds, utilisez la commande suivante :
```bash
npx sequelize-cli db:seed:undo:all
````