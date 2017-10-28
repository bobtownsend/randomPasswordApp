# README.md
How to setup Heroku

Heroku needs your project to have a Git repository, so we’ll create one along with a .gitignore file to ignore node_modules, and then commit the code:

$ git init
$ echo node_modules > .gitignore
$ git add .
$ git commit -m "Initial commit"
Now we’re ready for Heroku. Run its ‘create’ command:

$ heroku create

To make it work, we just need to push up our code by running:

$ git push heroku master

It will print out a bunch of stuff, and then the app will be live. One of the last lines will tell you the URL of the app

Now you can go to yoururl/api/passwords and make sure it works.