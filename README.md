# Projet 7 OpenClassrooms
	

![Vue.js](https://img.shields.io/badge/vuejs-framework%20frontend-green)
![TailwindCSS](https://img.shields.io/badge/Tailwind-framework%20CSS-blue)
![Sequelize](https://img.shields.io/badge/sequelise-ORM-informational)
![Express.js](https://img.shields.io/badge/Express.js-Applications--Web-9cf)
![NodeJS](https://img.shields.io/badge/Node--JS-environnement%20d'ex%C3%A9cution%20JavaScript-yellowgreen)

Parcours WebDev
Création d'un réseau social d'entreprise en se basant sur l'usage d'un framework et des compétances acquises tout le long du parcours. 

 
# Voici les exigences émises par le comité de pilotage :

* la présentation des fonctionnalités doit être simple ;
* la création d’un compte doit être simple et possible depuis un téléphone mobile ;
* le profil doit contenir très peu d’informations pour que sa complétion soit rapide ;
* la suppression du compte doit être possible ;
* l’accès à un forum où les salariés publient des contenus multimédias doit être présent ;
* l’accès à un forum où les salariés publient des textes doit être présent ;
* les utilisateurs doivent pouvoir facilement repérer les dernières participations des employés ;
* le ou la chargé-e de communication Groupomania doit pouvoir modérer les interactions entre
salariés ;

# Installation  
***
Clonez le repo : `https://github.com/services-web/f_joanan_7_052022` 

#### Pour lancer le frontend : 
* Placez vous dans le dossier frontend
* Dans le terminal exécutez la commande `npm install`
* Lancez ensuite la commande `npm run serve`
* L'interface client est disponible à l'URL suivante : http://localhost:8080/

#### Pour le backend suivez ces instructions :
* Placez vous dans le dossier backend
* Initialisez les packages via la commande `npm install`
* Lancez le backend en tapant ensuite `nodemon`
* Vérifiez bien que le backend communique via le port `:3000`

#### Mettez en place la base de données de cette manière :
* Connectez vous au serveur MySQL
* Lancez la commande suivante pour créer la base de données : `CREATE DATABASE groupomania`
* Vérifiez que vos identifiants de base de données correspondent avec ceux renseignés dans le fichier .env disponible dans le dossier Backend. Dans le cas échéant modifiez les au sein du fichier
* Importez enfin le fichier .sql disponible dans le dossier DB du Backend en tapant la commande suivante : `mysql -u votreidentifiant -p groupomania < sauvegarde.sql`

#### Enfin vous pouvez accèder à l'application ! 
* Lancez la via http://localhost:8080/
* Un compte admin est déjà disponible, connectez-vous avec l'identifiant `Admin`et le mot de passe `JeF12mql!`
