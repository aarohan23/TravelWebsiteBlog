# AngularMySql

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.7.3.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `-prod` flag for a production build.


## Setup

Download project and install the required node modules for frontend and backend :-

- navigate to root folder : Travel-Blog-Website and run ng install
- navigate to backend folder : backend and run node install

Download MySQL instance and and setup the database with following :-

var connection = mysql.createConnection({
	host: 'localhost',
	user: 'root',
	password: '',
	database: 'webpackcli'
});


CREATE TABLE IF NOT EXISTS `users` (

  `id` int(11) NOT NULL AUTO_INCREMENT,
  `username` varchar(30) NOT NULL,
  `password` varchar(255) NOT NULL,
  `email` varchar(100) NOT NULL,
  PRIMARY KEY (`username`),
  UNIQUE KEY `user_id` (`id`)
  
) 


CREATE TABLE IF NOT EXISTS `posts` (

  `id` int(11) NOT NULL AUTO_INCREMENT,
  `user_id` int(11) NOT NULL,
  `title` varchar(250) DEFAULT NULL,
  `destination` varchar(250) DEFAULT NULL,
  `experience` varchar(4000) DEFAULT NULL,
  `imagepath` varchar(250) DEFAULT NULL,
  PRIMARY KEY (`id`),
  KEY `user_id` (`user_id`)
  
)

- XAMMP Server with MySQL was used by me

## Running Travel-Blog-Website

- navigate to root folder : Travel-Blog-Website and run ng serve

This will run the Frontend on localhost:4200

- navigate to backend folder : backend and run node server

This will run the Backend on localhost:3000

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
# TravelWebsiteBlog
