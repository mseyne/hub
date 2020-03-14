# Template WordPress

Template pour démarrer une nouveau projet WordPress avec composer.

WP Starter = Wordpress + Composer est utilisé :
> https://wecodemore.github.io/wpstarter/

## Méthodologie

### 1. INSTALLATION DEV :

Cloner ce repo gitlab et lancer cette commande :

`composer install`

Créer le fichier de configuration .env avec les données correctes * :

```
WORDPRESS_ENV=development
DB_NAME=myprojectdatabase
DB_USER=myusername
DB_PASSWORD=motdepassedb *
WP_HOME=urlvhost *
```

pour la mise en production 

```
remplacer : WORDPRESS_ENV=production
ajouter :
DB_HOST=host
```

### 2. INSTALLATION FRONTEND :

* grunt, gulp ou npm runner à configurer pour sass, typescript, etc...

(le dossier node_modules sera ignoré par git en mettant à jour le .gitignore avec wp-content/themes/mon_theme/)

### 3. PLUGINS :

Plugins livré avec wpackagist.

* wp super cache : https://fr.wordpress.org/plugins/wp-super-cache/

### 4. préparation pour MISE EN PRODUCTION :

* Récupérer BD locale et dossier wp-content/uploads


Plus d'infos :
* https://wpackagist.org/  
* https://composer.rarst.net/
* https://github.com/Koodimonni/Composer-Dropin-Installer

Les dépendances de wp-starter :
* https://github.com/johnpbloch/wordpress
* https://github.com/vlucas/phpdotenv

Ajouter des langues :
* https://wp-languages.github.io

Underscores Theme : 
* http://underscores.me/
* https://themeshaper.com/2012/02/13/introducing-the-underscores-theme/