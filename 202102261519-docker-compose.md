# Docker Compose

#devops #docker #outils

CLI permettant de gérer plusieurs images à la fois dans un fichier YAML.

Syntaxe pour créer et démarrer les conteneurs définis dans un fichier spécifique :

```shell
docker-compose -f FILE up
```

## Exemple

```yaml
version: '3'
# Définit les N conteneurs à créer à partir de N images
services:
	mysql:
		container_name: boutique-lyf
		image: mysql
		environment:
			MYSQL_ROOT_PASSWORD: appmobile
		ports:
			- 3306:3306
```
