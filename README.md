# Deploying a Silex application on Heroku
After seeing a tweet by @hochchristoph, regarding his [heroku-buildpack-php](https://github.com/CHH/heroku-buildpack-php) released just a few days ago, I decided to build a sample application to test the process of deploying a Silex app to Heroku.

## Requirements
You'll need a couple of things before you can deploy your app :
* A Heroku account ([Signup on Heroku](https://id.heroku.com/signup))
* The Heroku Toolbelt for the CLI commands ([Download the Toolbelt](https://toolbelt.heroku.com/))

## Try it with this repo
* Clone this repo on your machine with `git clone https://github.com/marcaube/silex-heroku-hello.git silex-heroku-hello`
* Create your Heroku app with `heroku apps:create your-app-name --buildpack https://github.com/CHH/heroku-buildpack-php`
* Deploy with `git push heroku master`
* You're done!

## Start from scratch
* Create a new Silex app via Composer ([Install Silex](http://silex.sensiolabs.org/download))
* Create a git repo with `git init`
* Create a `.gitignore` file and add `/vendor/` and `/composer.phar`
* Add all other files with `git add .`
* Commit your changes `git commit -m "Initial commit"`
* Create your Heroku app with `heroku apps:create your-app-name --buildpack https://github.com/CHH/heroku-buildpack-php`
* Deploy with `git push heroku master`
* You're done!

## Going further
You can do the same with a Symfony app or with straight PHP, you can read more on this in the [heroku-buildpack-php docs](https://github.com/CHH/heroku-buildpack-php).
