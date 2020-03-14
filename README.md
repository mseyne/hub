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
DB_NAME=wp_suprameca
DB_USER=dev
DB_PASSWORD=motdepassedb *
WP_HOME=urlvhost *
```

pour la mise en production 

```
remplacer : WORDPRESS_ENV=production
ajouter :
DB_HOST=host
```

### 2. INSTALLATION INTE :

* Copier l'intégration dans le dossier assets du thème.
* Puis npm install et grunt compile/watch dans ce même dossier.

(le dossier node_modules sera ignoré par git en mettant à jour le .gitignore avec wp-content/themes/mon_theme/assets)

### 3. PLUGINS :

Plugins livré avec wpackagist :
*
*

Plugins externes à ajouter :
* Advanced Custom Fields Multilingual
* Advanced Custom Fields PRO
* Gravity Forms
* Gravity Forms Multilingual
* WPML Multilingual CMS
* WPML String Translation
* WPML Translation Management
* Yoast SEO
* Yoast SEO Multilingual | VestaThemes.com
* Ultimate GDPR

### 4. préparation pour MISE EN PRODUCTION :

* Récupérer BD locale et dossier wp-content/uploads
* Suivre procédures wiki pour config serveur, runner et gitlab


Plus d'infos :
* https://wpackagist.org/  
* https://composer.rarst.net/
* https://github.com/Koodimonni/Composer-Dropin-Installer

Les dépendances de wp-starter :
* https://github.com/johnpbloch/wordpress
* https://github.com/vlucas/phpdotenv

Plugins :
* wp super cache : https://fr.wordpress.org/plugins/wp-super-cache/

Ajouter des langues :
* https://wp-languages.github.io

Underscores Theme : 
* http://underscores.me/
* https://themeshaper.com/2012/02/13/introducing-the-underscores-theme/